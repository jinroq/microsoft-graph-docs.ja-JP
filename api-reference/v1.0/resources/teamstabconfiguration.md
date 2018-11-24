# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="cd6d0-101">teamsTabConfiguration リソースの種類 (オープン型)</span><span class="sxs-lookup"><span data-stu-id="cd6d0-101">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="cd6d0-102">[タブ](teamstab.md)の内容を決定する設定です。タブが対話形式で構成されている場合、この情報は、タブ プロバイダー アプリケーションによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="cd6d0-102">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="cd6d0-103">に加えて、以下のプロパティは、タブ プロバイダー アプリケーションをいくつかは、追加のカスタム プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="cd6d0-103">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="cd6d0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd6d0-104">Properties</span></span>

|<span data-ttu-id="cd6d0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd6d0-105">Property</span></span>|<span data-ttu-id="cd6d0-106">型</span><span class="sxs-lookup"><span data-stu-id="cd6d0-106">Type</span></span>|<span data-ttu-id="cd6d0-107">説明</span><span class="sxs-lookup"><span data-stu-id="cd6d0-107">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="cd6d0-108">エンティティ Id</span><span class="sxs-lookup"><span data-stu-id="cd6d0-108">entityId</span></span>   |   <span data-ttu-id="cd6d0-109">文字列</span><span class="sxs-lookup"><span data-stu-id="cd6d0-109">string</span></span> |  <span data-ttu-id="cd6d0-110">タブ プロバイダーによってホストされているエンティティの識別子です。</span><span class="sxs-lookup"><span data-stu-id="cd6d0-110">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="cd6d0-111">contentUrl</span><span class="sxs-lookup"><span data-stu-id="cd6d0-111">contentUrl</span></span> |   <span data-ttu-id="cd6d0-112">文字列</span><span class="sxs-lookup"><span data-stu-id="cd6d0-112">string</span></span> |  <span data-ttu-id="cd6d0-113">チームでのタブの内容を表示するために使用される Url です。</span><span class="sxs-lookup"><span data-stu-id="cd6d0-113">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="cd6d0-114">必須。</span><span class="sxs-lookup"><span data-stu-id="cd6d0-114">Required.</span></span>    |
|  <span data-ttu-id="cd6d0-115">removeUrl</span><span class="sxs-lookup"><span data-stu-id="cd6d0-115">removeUrl</span></span>  |   <span data-ttu-id="cd6d0-116">文字列</span><span class="sxs-lookup"><span data-stu-id="cd6d0-116">string</span></span> |  <span data-ttu-id="cd6d0-117">チームのクライアントを使用してタブが削除されたときに、チーム クライアントによって呼び出される Url。</span><span class="sxs-lookup"><span data-stu-id="cd6d0-117">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="cd6d0-118">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="cd6d0-118">websiteUrl</span></span> |   <span data-ttu-id="cd6d0-119">文字列</span><span class="sxs-lookup"><span data-stu-id="cd6d0-119">string</span></span> |  <span data-ttu-id="cd6d0-120">チーム以外のタブの内容を表示するための Url です。</span><span class="sxs-lookup"><span data-stu-id="cd6d0-120">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="cd6d0-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cd6d0-121">JSON representation</span></span>

<span data-ttu-id="cd6d0-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cd6d0-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
