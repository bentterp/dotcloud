Cloudfarm
=========

This project is intented to be a place for learning. The site was built to be used as an example of 
how a site can be developed, deployed and operated.

The site is based on .NET Core with ASP.NET Frmaework

Working style
=============

All sourcecode is kept in Git. and we try to adhere to the working model as describe  [here](http://nvie.com/posts/a-successful-git-branching-model/ "A successful Git branching model")

### Packet handling

All external packages should be installed using NuGet. Client dependencies should be installed using Bower or Gulp. Packages are *not* stored as part of this repository but are auto-installed by if they don't exist.

This means that the first time the project is built it will take some time to download all external packages.

## Deployment

This site is operated as a Web App in Microsoft Azure. The Web App consists of a IIS as a Service and a Azure SQL database.

Automatic publishing of code is setup as follows:

<table>
<tr>
<th>
Git branch
</th>
<th>Database</th>
<th>URL</th>
</tr>
<tr>
<td>develop</td>
<td>(localdb)\\mssqllocaldb</td>
<td>http://kbv-dev.azurewebsites.net</td>
</tr>
<tr>
<td>master</td>
<td>kontroll</td>
<td>http://kbv-prod.azurewebsites.net</td>
</tr>
</table>

### Deploy to production
TBD


# dotcloud
