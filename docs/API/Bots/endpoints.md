## Get bots
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/bots</span>
    </div>
    <span class="http-method-description">Returns all bots</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">List[Bot]</span>
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

## Get bot
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/bots/<strong>:bot_id</strong></span>
    </div>
    <span class="http-method-description">Returns a bot with specified id</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">Bot</span>
    </span>
</div>

## Get bot stats
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/bots/<strong>:bot_id</strong>/stats</span>
    </div>
    <span class="http-method-description">Returns bot stat records</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">List[BotStat]</span>
    </span>
</div>

## Get last bot stat
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-get-text http-method-text">GET</span>
        <span>/bots/<strong>:bot_id</strong>/stat</span>
    </div>
    <span class="http-method-description">Returns last bot stats record</span>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">BotStat</span>
    </span>
</div>

## Post bot stats
<div class="http-method">
    <div class="http-method-header">
        <span class="http-method-post-text http-method-text">POST</span>
        <span>/bots/<strong>:bot_id</strong>/stats</span>
    </div>
    <span class="http-method-response-model">
        <strong>Response model: </strong> 
        <span class="http-method-response-model-value">BotStat</span>
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
            <td>API key of these bot</td>
        </tr>
    </table>
    <h3 style="margin: 0">Request model</h3>
    <table>
        <thead>
            <tr>
                <th>Field</th>
                <th>Type</th>
                <th>Description</th>
            </tr>
        </thead>
        <tr>
            <td>users</td>
            <td>integer</td>
            <td>Count of bot users</td>
        </tr>
        <tr>
            <td>guilds</td>
            <td>integer</td>
            <td>Count of bot guilds</td>
        </tr>
        <tr>
            <td>shards</td>
            <td>integer?</td>
            <td>Count of bot shards</td>
        </tr><tr>
            <td>memory_load</td>
            <td>integer?</td>
            <td>The % of memory that is in use.</td>
        </tr>
        <tr>
            <td>cpu_load</td>
            <td>integer?</td>
            <td>The % of cpu that is in use.</td>
        </tr>
        <tr>
            <td>commands_executed</td>
            <td>integer?</td>
            <td>Count of number executed commands</td>
        </tr>
        <tr>
            <td>custom</td>
            <td>List[BotStatCustomField]?</td>
            <td>Custom data</td>
        </tr>
    </table>
</div>