# Obtaining the Model SPI

You can obtain the home object for the outbound HTTP connection configuration model by using JNDI lookup.

Here is a sample code snippet:

```
import com.ibm.portal.outbound.config.*;
...

javax.naming.Context ctx = new javax.naming.InitialContext();
OutboundConnectionModelHome home = (OutboundConnectionModelHome)   
            ctx.lookup("portal:service/model/OutboundConnectionModel");
OutboundConnectionModel model = home.getOutboundConnectionModelProvider().
                                GetOutboundConnectionModel();
```

The code that calls the SPI must run in the context of the portal server.


???+ info "Related information"  
    -   [Model SPI overview](../../../../../../../extend_dx/apis/model_spi/index.md)

