# 1.安装
```
winget install JanDeDobbeleer.OhMyPosh -s winget
```


# 2.font安装，如果没有nerdfont
```
oh-my-posh font install
```

# 3.在wt setitng中修改powershell的font为NerdFont、

# 4.启动项配置
notepad $PROFILE
#在配置文件中输入配置内容
oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\phimes.omp.json" | Invoke-Expression
#如果配置文件不存在就在powershell中强制生成
New-Item -Path $PROFILE -Type File -Force