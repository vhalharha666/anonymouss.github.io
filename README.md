#### basic configuration
my gye your nock at my door iwill open reach off folow reaper a gona take cover from neck offence to you and make the butchery at birth from your NAuthority
- install hexo: `npm install hexo -g`
- init project: `hexo init`
- intall dependencies: `npm install`
- config deployment: modify `_config.yml`
```yml
deploy:
  type: git
  repository: https://github.com/anonymouss/anonymouss.github.io.git
  branch: master
```
- install deploy ext: `npm install hexo-deployer-git --save`
- deploy: `hexo d -g`

#### theme

Next: `git clone https://github.com/theme-next/hexo-theme-next themes/next`

#### references

- Hexo: https://hexo.io/zh-cn/docs/configuration
- Next: http://theme-next.iissnan.com/getting-started.html

#### notes

> themes/next 's .git folder is removed, don't make it as git submodule

- config files in branch `hexo-config`
- blog static files in branch `master`

## switch to a new machine

- `git clone https://github.com/anonymouss/anonymouss.github.io.git`
- `cd anonymouss.github.io`
- `git checkout hexo-config`
- `npm install hexo -g`
- `npm install`
- `npm install hexo-deployer-git --save`
- make changes
- `./deploy.sh` # Hexo automatically commit to branch master
