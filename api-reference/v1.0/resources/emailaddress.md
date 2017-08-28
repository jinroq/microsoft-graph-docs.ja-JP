# <a name="emailaddress-resource-type"></a><span data-ttu-id="7b41e-101">emailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7b41e-101">emailAddress resource type</span></span>

<span data-ttu-id="7b41e-102">連絡先またはメッセージ受信者の名前と電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="7b41e-102">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="7b41e-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b41e-103">Properties</span></span>
| <span data-ttu-id="7b41e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b41e-104">Property</span></span>     | <span data-ttu-id="7b41e-105">型</span><span class="sxs-lookup"><span data-stu-id="7b41e-105">Type</span></span>   |<span data-ttu-id="7b41e-106">説明</span><span class="sxs-lookup"><span data-stu-id="7b41e-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b41e-107">address</span><span class="sxs-lookup"><span data-stu-id="7b41e-107">address</span></span>|<span data-ttu-id="7b41e-108">String</span><span class="sxs-lookup"><span data-stu-id="7b41e-108">String</span></span>|<span data-ttu-id="7b41e-109">個人またはエンティティの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="7b41e-109">The email address of the person or entity.</span></span>|
|<span data-ttu-id="7b41e-110">name</span><span class="sxs-lookup"><span data-stu-id="7b41e-110">name</span></span>|<span data-ttu-id="7b41e-111">String</span><span class="sxs-lookup"><span data-stu-id="7b41e-111">String</span></span>|<span data-ttu-id="7b41e-112">個人またはエンティティの表示名。</span><span class="sxs-lookup"><span data-stu-id="7b41e-112">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b41e-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b41e-113">JSON representation</span></span>

<span data-ttu-id="7b41e-114">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7b41e-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
