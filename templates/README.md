## Hi there :wave:

System administrator and web developer.

I write articles on system administration and development of various systems, applications and servers.

#### :construction_worker_man: I'm currently working on...

{{ range recentContributions 5 }}
- [{{ .Repo.Name }}]({{ .Repo.URL }}) ({{ humanize .OccurredAt }}){{ with .Repo.Description }}  
  {{ . }}{{ end }}
{{- end}}

#### :telescope: Recent releases

{{ range recentReleases 5 }}
- [{{ .Name }}]({{ .URL }}) ([{{ .LastRelease.TagName }}]({{ .LastRelease.URL }}), {{ humanize .LastRelease.PublishedAt }}){{ with .Description }}  
  {{ . }}{{ end }}
{{- end}}

#### :hammer: Recent pull requests

{{ range recentPullRequests 5 }}
- [{{ .Title }}]({{ .URL }}) ({{ humanize .CreatedAt }}) `{{ .State }}`  
  &#8627; [{{ .Repo.Name }}]({{ .Repo.URL }})
{{- end}}

#### :star: Recent stars

{{ range recentStars 5 }}
- [{{ .Repo.Name }}]({{ .Repo.URL }}) ({{ humanize .StarredAt }}){{ with .Repo.Description }}  
  {{ . }}{{ end }}
{{- end }}

#### :busts_in_silhouette: Recent followers

{{ range followers 5 }}
- [{{ with .Name }}{{ . }}{{ else }}{{ .Login }}{{ end }}]({{ .URL }})
{{- end }}

## Blog

{{ range rss "https://lib.onl/ru/posts/index.xml" 10 }}
- [{{ .Title }}]({{ .URL }}) ({{ humanize .PublishedAt }})
{{- end}}

## Projects

<img align="right" src="https://raw.githubusercontent.com/z17cx/z17cx/main/img.octocat.gif" width="20%" alt="OctoCat" />

- [**GitHub Package Store**](https://github.com/pkgstore)  
  Development storage for CMS/CMF, Linux OS and other various systems.
- [GitHub Actions Store](https://github.com/ghastore)  
  GitHub Actions makes it easy to automate all software workflows, now with world-class CI/CD.
- [GitHub Universal AIK](https://github.com/uaik)  
  (UNIX / Linux / Windows) automated installation kit.
