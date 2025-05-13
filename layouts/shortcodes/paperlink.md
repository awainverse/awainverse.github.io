{{ with (site.GetPage (print "research/" (.Get "paper"))) }}
- [{{ .Title }}]({{ .Permalink }})
{{ end }}