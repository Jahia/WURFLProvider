WURFLProvider
=============

The WURFLProvider module is an implementation of the WURFL library integration for resolving channels on a Jahia 6.6+ server

IMPORTANT:

In order to use this module, you will first need to download the latest WURFL database into the src/main/webapp/WEB-INF
directory and adjust the path to it in src/main/webapp/META-INF/spring/mod-wurfl in the following XML value:

    <bean id="wurflModel" class="net.sourceforge.wurfl.spring.SpringWURFLModel">
        <!--default root file location-->
        <property name="wurfl" value="/modules/wurfl-provider/WEB-INF/wurfl-VERSION.zip"/>

You can download the WURFL database zip file from the following location:

http://wurfl.sourceforge.net

and save into the src/main/webapp/WEB-INF directory (by creating it as it doesn't exist by default).

Unfortunately we cannot distribute this file in the module since the license for the database ZIP file is restrictive so
this is why this step is needed.
