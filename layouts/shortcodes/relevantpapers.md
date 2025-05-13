{{ with .Page.Params.papers }}
##### Relevant Papers

{{ range . }}
{{ with (site.GetPage (print "research/" . )) }}
- [{{ .Title }}]({{ .Permalink }})
{{ end }}
{{ end }}

---
    
{{ end }}