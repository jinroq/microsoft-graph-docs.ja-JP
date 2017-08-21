# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="34745-101">scoredEmailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34745-101">scoredEmailAddress resource type</span></span>

<span data-ttu-id="34745-102">スコアの付いたメール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="34745-102">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="34745-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34745-103">Properties</span></span>
| <span data-ttu-id="34745-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34745-104">Property</span></span>     | <span data-ttu-id="34745-105">型</span><span class="sxs-lookup"><span data-stu-id="34745-105">Type</span></span>   |<span data-ttu-id="34745-106">説明</span><span class="sxs-lookup"><span data-stu-id="34745-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34745-107">address</span><span class="sxs-lookup"><span data-stu-id="34745-107">address</span></span>|<span data-ttu-id="34745-108">string</span><span class="sxs-lookup"><span data-stu-id="34745-108">string</span></span>|<span data-ttu-id="34745-109">電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="34745-109">The user's email address.</span></span>|
|<span data-ttu-id="34745-110">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="34745-110">relevanceScore</span></span>|<span data-ttu-id="34745-111">double</span><span class="sxs-lookup"><span data-stu-id="34745-111">double</span></span>|<span data-ttu-id="34745-p101">電子メール アドレスの関連性スコア。関連性スコアは他の返された結果に関連して、並べ替えキーとして使用されます。関連性スコア値が高いほど、関連性の高い結果に対応します。関連性は、ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決定されます。</span><span class="sxs-lookup"><span data-stu-id="34745-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="34745-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34745-116">JSON representation</span></span>

<span data-ttu-id="34745-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="34745-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
