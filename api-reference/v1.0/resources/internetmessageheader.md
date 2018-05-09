# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="635df-101">internetMessageHeader リソースの種類</span><span class="sxs-lookup"><span data-stu-id="635df-101">internetMessageHeader resource type</span></span>


<span data-ttu-id="635df-102">[RFC5322](https://www.ietf.org/rfc/rfc5322.txt) によって定義された、インターネット メッセージ ヘッダーを表すキーと値のペア。メッセージが送信者から受信者に到達するまでに辿ったネットワーク パスの詳細を説明します。</span><span class="sxs-lookup"><span data-stu-id="635df-102">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="635df-103">インターネット メッセージ ヘッダーの例については、「[View e-mail message headers (電子メールのメッセージ ヘッダーを表示する)](https://support.office.com/ja-JP/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="635df-103">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/ja-JP/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="635df-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="635df-104">Properties</span></span>
| <span data-ttu-id="635df-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="635df-105">Property</span></span>     | <span data-ttu-id="635df-106">型</span><span class="sxs-lookup"><span data-stu-id="635df-106">Type</span></span>   |<span data-ttu-id="635df-107">説明</span><span class="sxs-lookup"><span data-stu-id="635df-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="635df-108">name</span><span class="sxs-lookup"><span data-stu-id="635df-108">name</span></span>|<span data-ttu-id="635df-109">string</span><span class="sxs-lookup"><span data-stu-id="635df-109">string</span></span>|<span data-ttu-id="635df-110">キーと値のペアの、キーの部分を表します。</span><span class="sxs-lookup"><span data-stu-id="635df-110">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="635df-111">value</span><span class="sxs-lookup"><span data-stu-id="635df-111">value</span></span>|<span data-ttu-id="635df-112">string</span><span class="sxs-lookup"><span data-stu-id="635df-112">string</span></span>|<span data-ttu-id="635df-113">キーと値のペアの、値の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="635df-113">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="635df-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="635df-114">JSON representation</span></span>

<span data-ttu-id="635df-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="635df-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->