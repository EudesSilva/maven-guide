
#maven-guide


![alt text](https://maven.apache.org/images/maven-logo-black-on-white.png "Maven")

What is the POM?

POM stands for "Project Object Model". It is an XML representation of a Maven project held in a file named pom.xml. When in the presence of Maven folks, speaking of a project is speaking in the philosophical sense, beyond a mere collection of files containing code. A project contains configuration files, as well as the developers involved and the roles they play, the defect tracking system, the organization and licenses, the URL of where the project lives, the project's dependencies, and all of the other little pieces that come into play to give code life. It is a one-stop-shop for all things concerning the project. In fact, in the Maven world, a project need not contain any code at all, merely a `pom.xml`.


#Quick Overview

This is a listing of the elements directly under the POM's project element. Notice that modelVersion contains 4.0.0. That is currently the only supported POM version for both Maven 2 & 3, and is always required.

 ```xml

    <project xmlns="http://maven.apache.org/POM/4.0.0"
      xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xsi:schemaLocation="http://maven.apache.org/POM/4.0.0
                          http://maven.apache.org/xsd/maven-4.0.0.xsd">
      <modelVersion>4.0.0</modelVersion>
     
      <!-- The Basics -->
      <groupId>...</groupId>
      <artifactId>...</artifactId>
      <version>...</version>
      <packaging>...</packaging>
      <dependencies>...</dependencies>
      <parent>...</parent>
      <dependencyManagement>...</dependencyManagement>
      <modules>...</modules>
      <properties>...</properties>
     
      <!-- Build Settings -->
      <build>...</build>
      <reporting>...</reporting>
     
      <!-- More Project Information -->
      <name>...</name>
      <description>...</description>
      <url>...</url>
      <inceptionYear>...</inceptionYear>
      <licenses>...</licenses>
      <organization>...</organization>
      <developers>...</developers>
      <contributors>...</contributors>
     
      <!-- Environment Settings -->
      <issueManagement>...</issueManagement>
      <ciManagement>...</ciManagement>
      <mailingLists>...</mailingLists>
      <scm>...</scm>
      <prerequisites>...</prerequisites>
      <repositories>...</repositories>
      <pluginRepositories>...</pluginRepositories>
      <distributionManagement>...</distributionManagement>
      <profiles>...</profiles>
    </project>
``` 
    
    
#Documentation oficial 
[Oficial maven!](https://maven.apache.org/guides/index.html)


<h3><a name="Getting_Started_with_Maven"></a>Getting Started with Maven</h3>
<ul>
<li><a href="https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html">Getting Started in 5 Minutes</a></li>
<li><a href="https://maven.apache.org/guides/getting-started/index.html">Getting Started in 30 Minutes</a></li></ul></div>
<div class="section">
<h3><a name="Introductions"></a>Introductions</h3>
<ul>
<li><a href="https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html">The Build Lifecycle</a></li>
<li><a href="https://maven.apache.org/guides/introduction/introduction-to-the-pom.html">The POM</a></li>
<li><a href="https://maven.apache.org/guides/introduction/introduction-to-profiles.html">Profiles</a></li>
<li><a href="https://maven.apache.org/guides/introduction/introduction-to-repositories.html">Repositories</a></li>
<li><a href="https://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html">Standard Directory Layout</a></li>
<li><a href="https://maven.apache.org/guides/introduction/introduction-to-dependency-mechanism.html">The Dependency Mechanism</a></li>
<li><a href="https://maven.apache.org/guides/introduction/introduction-to-optional-and-excludes-dependencies.html"> Optional Dependencies and Dependency Exclusions</a></li></ul>
<div class="section">
<h4><a name="Plugins"></a>Plugins</h4>
<ul>
<li><a href="https://maven.apache.org/guides/introduction/introduction-to-plugins.html">Plugin Development</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-configuring-plugins.html">Configuring Plug-ins</a></li>
<li><a href="https://maven.apache.org/guides/introduction/introduction-to-plugin-prefix-mapping.html">Plugin Prefix Resolution</a></li>
<li><a href="https://maven.apache.org/guides/plugin/guide-java-plugin-development.html">Developing Java Plugins</a></li></ul></div>
<div class="section">
<h4><a name="Site"></a>Site</h4>
<ul>
<li><a href="https://maven.apache.org/guides/mini/guide-site.html">Creating a Site</a></li>
<li><a class="externalLink" href="http://maven.apache.org/doxia/references/apt-format.html">The APT Format</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-snippet-macro.html">Snippet Macro</a></li></ul></div>
<div class="section">
<h4><a name="Archetypes"></a>Archetypes</h4>
<ul>
<li><a href="https://maven.apache.org/guides/introduction/introduction-to-archetypes.html">What is an Archetype</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-creating-archetypes.html">Creating Archetypes</a></li></ul></div>
<div class="section">
<h4><a name="Upgrading"></a>Upgrading</h4>
<ul>
<li><a href="https://maven.apache.org/guides/mini/guide-relocation.html">Relocation of Artifacts</a></li></ul></div>
<div class="section">
<h4><a name="Repositories"></a>Repositories</h4>
<ul>
<li><a href="https://maven.apache.org/guides/mini/guide-3rd-party-jars-local.html">Installing 3rd party JARs to Local Repository</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-3rd-party-jars-remote.html">Deploying 3rd party JARs to Remote Repository</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-coping-with-sun-jars.html">Coping with Sun JARs</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-repository-ssl.html">Remote repository access through authenticated HTTPS</a></li></ul></div></div>
<div class="section">
<h3><a name="Guides"></a>Guides</h3>
<ul>
<li><a href="https://maven.apache.org/guides/mini/guide-assemblies.html">Creating Assemblies</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-archive-configuration.html">Configuring Archive Plugins</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-configuring-maven.html">Configuring Maven</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-mirror-settings.html">Mirror Settings</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-deployment-security-settings.html">Deployment and Security Settings</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-generating-sources.html">Generating Sources</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-manifest.html">Working with Manifests</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-maven-classloading.html">Maven Classloading</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-multiple-modules.html">Using Multiple Modules in a Build</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-multiple-repositories.html">Using Multiple Repositories</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-proxies.html">Using Proxies</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-releasing.html">Using the Release Plugin</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-using-ant.html">Using Ant with Maven</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-using-modello.html">Using Modello</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-using-extensions.html">Using Extensions</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-building-for-different-environments.html">Building For Different Environments with Maven 2</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-using-toolchains.html">Using Toolchains</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-encryption.html"> Encrypting passwords in settings.xml</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-http-settings.html"> Guide to HTTP Connection Settings</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-wagon-providers.html"> Guide to Selecting Alternative Wagon Providers</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-building-jdk14-on-jdk15.html"> Guide to Building JDK 1.4 Projects Using JDK 1.5</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-default-execution-ids.html"> Guide to Configuring Default Mojo Executions</a></li></ul>
<div class="section">
<h4><a name="Maven_Tools_and_IDE_Integration"></a>Maven Tools and IDE Integration</h4>
<ul>
<li><a href="https://maven.apache.org/guides/mini/guide-bash-m2-completion.html">Maven Auto-Completion Using BASH</a></li></ul></div></div>
<div class="section">
<h3><a name="Development_Guides"></a>Development Guides</h3>
<ul>
<li><a href="https://maven.apache.org/guides/development/guide-building-maven.html">Building Maven from Scratch</a></li>
<li><a href="https://maven.apache.org/guides/development/guide-maven-development.html">Developing Maven</a></li>
<li><a href="https://maven.apache.org/guides/development/guide-plugin-documentation.html">The Plugin Documentation Standard</a></li>
<li><a href="https://maven.apache.org/guides/development/guide-documentation-style.html">Maven Documentation Style</a></li></ul></div>
<div class="section">
<h3><a name="The_Maven_Community"></a>The Maven Community</h3>
<ul>
<li><a href="https://maven.apache.org/community.html">The Maven Community</a></li>
<li><a href="https://maven.apache.org/guides/development/guide-helping.html">Helping with Maven</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-new-committers.html">Guide for New Committers</a></li>
<li><a href="https://maven.apache.org/guides/development/guide-testing-development-plugins.html">Testing Development Versions of Plugins</a></li>
<li><a href="https://maven.apache.org/articles.html">3rd Party Resources</a></li></ul>
<div class="section">
<h4><a name="Conventions"></a>Conventions</h4>
<ul>
<li><a href="https://maven.apache.org/maven-conventions.html">Maven Conventions</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-naming-conventions.html">Naming Conventions</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-using-one-source-directory.html">When You Can't Use the Conventions</a></li></ul></div>
<div class="section">
<h4><a name="The_Central_Repository"></a>The Central Repository</h4>
<ul>
<li><a href="https://maven.apache.org/guides/mini/guide-central-repository-upload.html">Uploading Artifacts to the Central Repository</a></li>
<li><a href="https://maven.apache.org/guides/mini/guide-maven-evangelism.html">Improving the Repository</a></li></ul></div></div>
<div class="section">
<h3><a name="References"></a>References</h3>
<ul>
<li><a href="https://maven.apache.org/pom.html">POM Overview</a> (<a href="https://maven.apache.org/ref/current/maven-model/maven.html">Technical Project Descriptor</a>)</li>
<li><a href="https://maven.apache.org/settings.html">Settings Overview</a> (<a href="https://maven.apache.org/ref/current/maven-settings/settings.html">Technical Settings Descriptor</a>)</li>
<li><a href="https://maven.apache.org/plugins/index.html">Core Plug-ins List</a></li>
<li><a href="https://maven.apache.org/developers/mojo-api-specification.html">Mojo API</a></li>
<li><a href="https://maven.apache.org/glossary.html">Glossary</a></li>
<li><a href="https://maven.apache.org/guides/MavenQuickReferenceCard.pdf">Maven Quick Reference Card - PDF</a></li></ul></div>
<div class="section">
<h3><a name="Javadoc_API"></a>Javadoc API</h3>
<p>Here is some useful Javadoc API links to the current version of Maven:</p>
<ul>
<li><a class="externalLink" href="http://maven.apache.org/ref/current/maven-artifact/apidocs/">Maven Artifact</a></li>
<li><a class="externalLink" href="http://maven.apache.org/shared/maven-reporting-api/apidocs/">Maven Reporting</a></li>
<li><a class="externalLink" href="http://maven.apache.org/ref/current/maven-plugin-api/apidocs/">Maven Plugin API</a></li>
<li><a class="externalLink" href="http://maven.apache.org/ref/current/maven-model/apidocs/">Maven Model</a></li>
<li><a class="externalLink" href="http://maven.apache.org/ref/current/maven-core/apidocs/">Maven Core</a></li>
<li><a class="externalLink" href="http://maven.apache.org/ref/current/maven-settings/apidocs/">Maven Settings</a></li></ul>
<p>You could also browse the <a class="externalLink" href="http://maven.apache.org/ref/current/">full technical documentation references</a> of the current version of Maven.</p>

 <p>Copyright �2002 � 2016
<a href="https://www.apache.org/">The Apache Software Foundation</a>.
All rights reserved.</p>

