# <a name="phone-resource-type"></a><span data-ttu-id="dfac5-101">電話リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfac5-101">phone resource type</span></span>

<span data-ttu-id="dfac5-102">電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="dfac5-102">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="dfac5-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfac5-103">Properties</span></span>
| <span data-ttu-id="dfac5-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfac5-104">Property</span></span>     | <span data-ttu-id="dfac5-105">型</span><span class="sxs-lookup"><span data-stu-id="dfac5-105">Type</span></span>   |<span data-ttu-id="dfac5-106">説明</span><span class="sxs-lookup"><span data-stu-id="dfac5-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfac5-107">number</span><span class="sxs-lookup"><span data-stu-id="dfac5-107">number</span></span>|<span data-ttu-id="dfac5-108">string</span><span class="sxs-lookup"><span data-stu-id="dfac5-108">string</span></span>|<span data-ttu-id="dfac5-109">電話番号。</span><span class="sxs-lookup"><span data-stu-id="dfac5-109">The phone number.</span></span>|
|<span data-ttu-id="dfac5-110">種類</span><span class="sxs-lookup"><span data-stu-id="dfac5-110">type</span></span>|<span data-ttu-id="dfac5-111">String</span><span class="sxs-lookup"><span data-stu-id="dfac5-111">String</span></span>|<span data-ttu-id="dfac5-p101">電話番号の種類。可能な値は、`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio` です。</span><span class="sxs-lookup"><span data-stu-id="dfac5-p101">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfac5-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfac5-114">JSON representation</span></span>

<span data-ttu-id="dfac5-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dfac5-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->