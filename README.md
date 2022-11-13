<img src="https://user-images.githubusercontent.com/66525257/201532176-31af4466-fa54-4ff9-84cc-28cc58c71fc5.jpg" width=600 />

友人への講義の出席依頼を Line Bot で自動化する

## Design

```sh
cmd
└── request_syspro_attendance_job # シスプロの出席を依頼するJob
    ├── main.go
    └── run.go
```

これらのエンドポイントを CloudRun へデプロイし、CloudScheduler で毎週の講義前に定期実行する。

- [📝 CloudRun & CloudScheduler Resources](https://github.com/search?q=repo%3Aigsr5%2Figsr5-terraform%20attendance_request_bot&type=code)

