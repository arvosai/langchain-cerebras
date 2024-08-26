# 🦜️🔗 LangChain {partner}

This repository contains 1 package with Cerebras integrations with LangChain:

- [langchain-cerebras](https://pypi.org/project/langchain-cerebras/)

## Initial Repo Checklist (Remove this section after completing)

This setup assumes that the partner package is already split. For those instructions,
see [these docs](https://python.langchain.com/docs/contributing/integrations#partner-packages).

Code

Workflow code

- [ ] Add secrets as env vars in .github/workflows/_release.yml

In github

- [ ] Add integration testing secrets in Github (ask Erick for help)
- [ ] Add partner collaborators in Github (ask Erick for help)
- [ ] "Allow auto-merge" in General Settings 
- [ ] Only "Allow squash merging" in General Settings
- [ ] Set up ruleset matching CI build (ask Erick for help)
    - name: ci build
    - enforcement: active
    - bypass: write
    - target: default branch
    - rules: restrict deletions, require status checks ("CI Success"), block force pushes

Pypi

- [ ] Add new repo to test-pypi and pypi trusted publishing (ask Erick for help)

Slack

- [ ] Set up release alerting in Slack (ask Erick for help)

release:
/github subscribe langchain-ai/langchain-{partner} releases workflows:{name:"release"}
/github unsubscribe langchain-ai/langchain-{partner} issues pulls commits deployments
