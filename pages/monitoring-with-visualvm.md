#Monitor applications with VisualVM

VisualVM is a graphical tool for viewing and monitoring the performance of Java applications running on JVM. 

If you have a JRuby application deployed on Engine Yard Cloud and you can monitor the application with VisualVM on your local machine. This page describes how.

**Note:** This procedure assumes that you have the JDK (Java Developers Kit) installed on your local machine. VisualVM is included in the JDK. 

##To monitor a JRuby application with VisualVM  



1. Deploy your JRuby application on Engine Yard Cloud. 
    **Note:** Set the runtime to JRuby 1.6.5 (ruby-1.8.7-p330). VisualVM is not compatible with Ruby 1.9.

2. Use rvm to open a JRuby development environment in your local machine.

3. In 




<h2 id="topic5"> More information</h2>

<table>
	  <tr>
	    <th>For more information about...</th><th>See...</th>
	  </tr>
	  <tr>
	    <td>connecting VisualVM with your Engine Yard Cloud application</td><td>[[VisualVM on Engine Yard Cloud|http://vimeo.com/33750907]].</td>
	  </tr> 
	 <tr>
	    <td>deploying a JRuby application on Engine Yard Cloud</td><td>[[Using JRuby on Engine Yard Cloud|deploy-jruby]].</td>
	  </tr>
	  <tr>
	    <td>how to use VisualVM</td><td>[[VisualVM documentation|http://visualvm.java.net/]].</td>
	  </tr>
</table>
