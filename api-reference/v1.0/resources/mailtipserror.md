# <a name="mailtipserror-resource-type"></a><span data-ttu-id="85926-101">mailTipsError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="85926-101">mailTipsError resource type</span></span>

<span data-ttu-id="85926-102">操作中に発生するエラーです。</span><span class="sxs-lookup"><span data-stu-id="85926-102">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="85926-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85926-103">Properties</span></span>
| <span data-ttu-id="85926-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85926-104">Property</span></span>     | <span data-ttu-id="85926-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="85926-105">Type</span></span>   |<span data-ttu-id="85926-106">説明</span><span class="sxs-lookup"><span data-stu-id="85926-106">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="85926-107">message</span><span class="sxs-lookup"><span data-stu-id="85926-107">message</span></span> | <span data-ttu-id="85926-108">文字列</span><span class="sxs-lookup"><span data-stu-id="85926-108">String</span></span> | <span data-ttu-id="85926-109">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="85926-109">The error message.</span></span> |
| <span data-ttu-id="85926-110">code</span><span class="sxs-lookup"><span data-stu-id="85926-110">code</span></span> | <span data-ttu-id="85926-111">文字列</span><span class="sxs-lookup"><span data-stu-id="85926-111">String</span></span> | <span data-ttu-id="85926-112">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="85926-112">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="85926-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="85926-113">JSON representation</span></span>

<span data-ttu-id="85926-114">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="85926-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->