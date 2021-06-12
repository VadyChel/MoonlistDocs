## Get servers
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/servers</span>
    </div>
    <span class="http-method-description">Returns all servers</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">List[Server]</span>
    </span>
    <h3 style="margin: 1em 0 0">Params</h3>
    <table>
        <thead>
            <tr>
                <th>Field</th>
                <th>Default</th>
                <th>Description</th>
            </tr>
        </thead>
        <tr>
            <td>limit</td>
            <td>20</td>
            <td>The limit number of the bots</td>
        </tr>
        <tr>
            <td>skip</td>
            <td>0</td>
            <td>The offset of the bots</td>
        </tr>
    </table>
</div>

## Get server
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/servers/<strong>:server_id</strong></span>
    </div>
    <span class="http-method-description">Returns a server with specified id</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">Server</span>
    </span>
</div>