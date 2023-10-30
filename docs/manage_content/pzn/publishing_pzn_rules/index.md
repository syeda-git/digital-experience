# Publishing personalization rules

HCL Digital Experience Personalization sends published rules across HTTP to a servlet which resides on each personalization server.

When a user begins a publishing job from the personalization authoring environment, the local servlet is provided with the set of information necessary to complete the job. The local servlet contacts the destination endpoint servlet (which could be the same servlet\) and sends its data to it. The destination servlet reports success or failure.

1.  [Publishing considerations](pzn_publish_considerations.md)  
Be familiar with unique publishing considerations if you are publishing to or from a clustered environment, IPv6 hots, or Resource collection classes.
2.  [Publishing personalization rules](pzn_publishing_objects.md)  
After developing personalization rules, you publish the rules.
3.  [Publishing and deleting personalization rules using a script](pzn_publish_script.md)  
You can use a HCL Digital Experience Personalization provided script, pznload, to export, publish, and delete Personalization rules on local or remote servers.
4.  [Publishing personalization rules over SSL](pzn_publish_secure.md)  
HCL Digital Experience Personalization uses the built-in SSL capabilities of WebSphere Application Server to provide secure publishing across unprotected networks.
5.  [Monitoring the status of publishing](pzn_publish_status.md)  
After you start a job to publish a personalization rule, you can monitor the status to make sure the publish completes successfully.


???+ info "Related information"  
    -   [Staging to production list](../../../deployment/manage/staging_to_production/overview_of_staging_to_prod/dep_stage_check.md)

