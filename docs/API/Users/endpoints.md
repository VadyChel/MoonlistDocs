## Get current user
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/users/@me</span>
    </div>
    <span class="http-method-description">Gets current user</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">User</span>
    </span>
</div>

## Get user
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/users/<strong>:user_id</strong></span>
    </div>
    <span class="http-method-description">Gets user with a specified id</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">User</span>
    </span>
</div>

## Get user bots
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/users/<strong>:user_id</strong>/bots</span>
    </div>
    <span class="http-method-description">Gets specified user bots</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">List[Bot]</span>
    </span>
</div>

## Get user servers
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/users/<strong>:user_id</strong>/servers</span>
    </div>
    <span class="http-method-description">Gets specified user servers</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">List[Server]</span>
    </span>
</div>

## Get user webhooks
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/users/<strong>:user_id</strong>/webhooks</span>
    </div>
    <span class="http-method-description">Gets specified user webhooks</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">List[Webhook]</span>
    </span>
    <h3 style="margin: 1em 0 0">Headers</h3>
    <table>
        <thead>
            <tr>
                <th>Field</th>
                <th>Type</th>
                <th>Description</th>
            </tr>
        </thead>
        <tr>
            <td>Authorization</td>
            <td>string</td>
            <td>Bearer {user token}</td>
        </tr>
    </table>
</div>