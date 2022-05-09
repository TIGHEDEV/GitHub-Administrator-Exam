<!-- ## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/TIGHEDEV/GitHub-Administrator-Exam/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/TIGHEDEV/GitHub-Administrator-Exam/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
-->
# GitHub Enterprise Revision guide

This revision guide is based off the content from the MS [Learn path:](https://docs.microsoft.com/en-us/learn/paths/github-administration-products/) and content from the learning paths at the following [site:](https://docs.microsoft.com/en-us/users/githubtraining/collections/mom7u1gzjdxw03)

## GitHub Administration

### Administration levels

1. Organisation
2. Teams - these can and should be nested
3. User

### Sync your GitHub team with your identity provider.

If using AzureAD, changes in AD will be reflected in GitHub.

### Organisation level administration

Organisation "owner" permissions allows you to do these activities:
- Invite and remove members from an organisation
- Place users into teams and grant "team maintaner" permissions to users
- Add or remover external collaborators
- Grant repository permission levels
- Set up organisation security
- Use customer scripts to get extra info from the repositories and apply migrations/organisation-wide changes.

## GitHub Authentication

### Authenitcation Options

1. Username and password
2. Personal Access Tokens
3. SSH Keys
4. Deploy Keys
5. MFA
6. SAML SSO (Security Assertion Markup Language)
7. LDAP (Lightweight Directory Access Protocol)

## GitHub Permissions

### Repository Permissions

- **Read** For people who need to see the code but not interact with it
- **Triage** For people who proactively manage issyes amd pull requests but do not need write permissions
- **Write** For the standard developer and people who actively contribute to your project
- **Maintain** For project managers. Does not provide access to sensitive or destruvtive actions
- **Admin** For people who need full access to the project

Repository permissions can be be applied to organisation members, external collaborators and teams. 

### Team permissions

Permissions will cascade through teams that have child teams. Therefore you can apply repository permissions to a parent team that will benfit child teams of that parent. Make sure to only apply the right level of permissions to the parent team and then be more specific with child team permissions.

- **Member** Same set of abilites as organisation members
- **Maintainer** Is a team admin essentially. Abilities include: request team change parent and child teams; edit team discussions; and and remove members; give maintatner permission to other users; manage access to repositories; manage code review assignment and scheduled reminders for pull requests. An organisation owner can also prmote someone to become a maintainer. 

### Organisation Permissions

- **Owner** Can add or remove users to and from the organisation and do everything organisation members can do.
- **Member** Can create and manage organisation repositories and teams.
- **Billing Manager** Can only view and edit billing information.

You can set default permissions for all members of your organisation.

### Enterprise Permissions

- **Owner** The ultimate admin, can do everything!
- **Member** Same as an organisation member.
- **Billing Manager** Can only view billing information and add other billing managers.




