# jgitflow-maven-plugin (example)

## Abstract


## Pre-requisites

## Description

## Flow

## settings.xml

	By default, Maven will search the groupId org.apache.maven.plugins for prefix-to-artifactId mappings 
	for the plugins it needs to perform a given build. However the user may have a need for third-party 
	plugins. Since the Maven project is assumed to have control over the default plugin groupId, 
	this means configuring Maven to search other groupId locations for plugin-prefix mappings.

	As it turns out, this is simple. In the Maven settings file (per-user: ~/.m2/settings.xml; 
	global: $M2_HOME/conf/settings.xml), or local (settings.xml) you can provide a custom pluginGroups 
	section, listing the plugin groupIds you want to search (each groupId goes in its own pluginGroup 
	sub-element). For example, if my project uses a jgitflow-maven-plugin, I might have the following in 
	my settings:
	
	```xml
	
		<pluginGroups>
			<pluginGroup>external.atlassian.jgitflow</pluginGroup>
		</pluginGroups>
	
	```
## Contact

Email: staleks@gmail.com
Webpage: staleks.github.io



