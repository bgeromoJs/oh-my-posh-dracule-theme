# oh-my-posh-dracule-theme


{
    "$schema": "https://raw.githubusercontent.com/JanDeDobbeleer/oh-my-posh/main/themes/schema.json",
    "blocks": [
      {
        "alignment": "left",
        "segments": [
          {
            "background": "#41ba60",
            "foreground": "#000",
            "leading_diamond": "\ue0b6",
            "style": "diamond",
            "template": "{{ .UserName }}@{{ .HostName }}",
            "trailing_diamond": "\ue0b0",
            "type": "session"
          },
          {
            "background": "#9da352",
            "foreground": "#000",
            "powerline_symbol": "\ue0b0",
            "properties": {
              "folder_icon": " \uf115 ",
              "folder_separator_icon": " \ue0b1 ",
              "style": "full"
            },
            "style": "powerline",
            "template": " {{ .Path }}",
            "type": "path"
          },
          {
            "background": "#802f5d",
            "foreground": "#000",
            "powerline_symbol": "\ue0b0",
            "style": "powerline",
            "template": " {{ .HEAD }} ",
            "type": "git"
          },
          {
            "background": "#906cff",
            "foreground": "#100e23",
            "powerline_symbol": "\ue0b0",
            "style": "powerline",
            "template": " \ue235 {{ if .Error }}{{ .Error }}{{ else }}{{ if .Venv }}{{ .Venv }} {{ end }}{{ .Full }}{{ end }} ",
            "type": "python"
          },
          {
            "background": "#ff8080",
            "foreground": "#ffffff",
            "powerline_symbol": "\ue0b0",
            "style": "powerline",
            "template": " \ue20f ",
            "type": "exit"
          }
        ],
        "type": "prompt"
      },
      {
        "alignment": "left",
        "newline": true,
        "segments": [
          {
            "foreground": "#007ACC",
            "style": "plain",
            "template": "\u276f ",
            "type": "text"
          }
        ],
        "type": "prompt"
      }
    ],
    "version": 2
}

