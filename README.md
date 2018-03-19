### Jupyterhub On Kubernetes

  这个是在kubernetes上面部署jupyterhub需要的配置文件，具体的安装文档可以在 https://oopsoh.github.io 文档里面找到，这些文件就是文档里面所用到的具体文件，你可以根据你的具体情况，去参考文档然后修改为你的实际配置。
  

- config.yaml: 使用helm安装的时候，指定的配置文档，用来覆盖安装软件的默认values.yaml中的默认值。
- basenotebookimage: 自定义base-notebook的docker镜像。
- hubldapimage: 自定义k8s-hub镜像，集成ldap验证的docker镜像。
- jupyterhub: 使用helm下载下来的Charts文件夹，有默认的安装到kubernetes上的yaml文件。
- singleuserimage: 自定义的每个用户启动notebook的docker镜像。
- jupyterhub-ingress-ui.yaml: 在kubernetes上面使用Ingress暴露jupyterhub web界面的yaml配置文件。
- claim-share.yaml: 在kubernetes上面创建用于pod之间的共享pvc。
