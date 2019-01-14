# github接入

## 步骤

1. 访问此页面 
    - [生成access访问码](http://39.105.183.116/debian/service-github.html)
2. 点击生成
    - ![点击生成](assets/2019-01-14-23-32-59.png)
3. 复制你的访问码
    - ![复制你的访问码](assets/2019-01-14-23-34-50.png)
4. 打开你需要接入的仓库页面,点击`settings`
    - ![settings](assets/2019-01-14-23-44-26.png)
5. 添加`webhoos`
    - ![webhoos](assets/2019-01-14-23-45-41.png)
6. 编辑webhooks的表单
    - ![表单](assets/2019-01-14-23-46-36.png)
    - Payload URL
      - 填写 `http://39.105.183.116/api/hooks/`+你的访问码
    - Content type
      - 填写 `application/json`
    - Secret
      - 随意 
    - Which events would you like to trigger this webhook?
      - 选择`Just the push event.`
7. 点击添加

8. 等待数秒查看网页即可

> 访问码用于确认属于你的唯一仓库