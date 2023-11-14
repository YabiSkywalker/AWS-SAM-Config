.Phony: build 

build: 
	sam build 

deploy-infra: 
	sam build && aws-vault exec my-user --no-session -- sam deploy 

deploy-site: 
	aws-vault exec my-user --no-session -- aws s3 sync ./myresumeyabi-1 s3://cloud-resume-yabi