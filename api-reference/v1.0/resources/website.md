# <a name="website-resource-type"></a><span data-ttu-id="5ddc7-101">Web サイトのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ddc7-101">website resource type</span></span>

<span data-ttu-id="5ddc7-102">Web サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="5ddc7-102">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="5ddc7-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ddc7-103">Properties</span></span>
| <span data-ttu-id="5ddc7-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ddc7-104">Property</span></span>     | <span data-ttu-id="5ddc7-105">型</span><span class="sxs-lookup"><span data-stu-id="5ddc7-105">Type</span></span>   |<span data-ttu-id="5ddc7-106">説明</span><span class="sxs-lookup"><span data-stu-id="5ddc7-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ddc7-107">type</span><span class="sxs-lookup"><span data-stu-id="5ddc7-107">type</span></span>|<span data-ttu-id="5ddc7-108">String</span><span class="sxs-lookup"><span data-stu-id="5ddc7-108">String</span></span>| <span data-ttu-id="5ddc7-109">可能な値は、`other`、`home`、`work`、`blog`、`profile` です。</span><span class="sxs-lookup"><span data-stu-id="5ddc7-109">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="5ddc7-110">アドレス</span><span class="sxs-lookup"><span data-stu-id="5ddc7-110">address</span></span>|<span data-ttu-id="5ddc7-111">string</span><span class="sxs-lookup"><span data-stu-id="5ddc7-111">string</span></span>|<span data-ttu-id="5ddc7-112">Web サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="5ddc7-112">The URL of the current website.</span></span>|
|<span data-ttu-id="5ddc7-113">displayName</span><span class="sxs-lookup"><span data-stu-id="5ddc7-113">displayName</span></span>|<span data-ttu-id="5ddc7-114">string</span><span class="sxs-lookup"><span data-stu-id="5ddc7-114">string</span></span>|<span data-ttu-id="5ddc7-115">Web サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="5ddc7-115">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ddc7-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ddc7-116">JSON representation</span></span>

<span data-ttu-id="5ddc7-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ddc7-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
