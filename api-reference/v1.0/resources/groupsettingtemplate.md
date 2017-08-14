<span data-ttu-id="97fcb-p102">テンプレートの一意識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97fcb-p102">Unique identifier for the subscription. Read-only.</span></span>| テンプレートの一意識別子です。読み取り専用です。|
|<span data-ttu-id="97fcb-131">値</span><span class="sxs-lookup"><span data-stu-id="97fcb-131">values</span></span>|<span data-ttu-id="97fcb-132">[settingTemplateValue](settingtemplatevalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="97fcb-132">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="97fcb-133">このテンプレートを構成する、一連の利用可能な設定、既定値、種類を一覧表示する settingTemplateValues のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="97fcb-133">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="97fcb-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97fcb-134">Relationships</span></span>

<span data-ttu-id="97fcb-135">なし。</span><span class="sxs-lookup"><span data-stu-id="97fcb-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="97fcb-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97fcb-136">JSON representation</span></span>

<span data-ttu-id="97fcb-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97fcb-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->