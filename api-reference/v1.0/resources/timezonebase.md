# <a name="timezonebase-resource-type"></a><span data-ttu-id="51a61-101">timeZoneBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="51a61-101">timeZoneBase resource type</span></span>

<span data-ttu-id="51a61-102">タイム ゾーンの基本的な表現です。</span><span class="sxs-lookup"><span data-stu-id="51a61-102">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="51a61-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51a61-103">Properties</span></span>
| <span data-ttu-id="51a61-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51a61-104">Property</span></span>     | <span data-ttu-id="51a61-105">型</span><span class="sxs-lookup"><span data-stu-id="51a61-105">Type</span></span>   |<span data-ttu-id="51a61-106">説明</span><span class="sxs-lookup"><span data-stu-id="51a61-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51a61-107">name</span><span class="sxs-lookup"><span data-stu-id="51a61-107">name</span></span> | <span data-ttu-id="51a61-108">string</span><span class="sxs-lookup"><span data-stu-id="51a61-108">string</span></span> | <span data-ttu-id="51a61-109">タイム ゾーンの名前。</span><span class="sxs-lookup"><span data-stu-id="51a61-109">The name of a time zone.</span></span> <span data-ttu-id="51a61-110">標準的なタイム ゾーンの名前 ("ハワイ アリューシャン標準時" など) を使用することも、カスタム タイム ゾーンとして "カスタム タイム ゾーン" という名前を指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="51a61-110">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="51a61-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51a61-111">JSON representation</span></span>

<span data-ttu-id="51a61-112">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="51a61-112">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->