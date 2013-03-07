webjars-locator
===============

This project provides a means to locate assets within WebJars.

Obtain the full path of an asset
--------------------------------

	WebJarAssetLocator locator = new WebJarAssetLocator();
	String fullPathToRequirejs = locator.getFullPath("require.js");
	
Obtain all of the assets within a base folder
---------------------------------------------
	
	WebJarAssetLocator locator = new WebJarAssetLocator();
	Set<String> fullPathsOfAssets = locator.listAssets("/multiple/1.0.0");

Advanced usage
--------------

The locator can also be configured with the class loaders that it should use for looking up resources and filter the types of resources that should be included for searching. Please visit the source code for more information.