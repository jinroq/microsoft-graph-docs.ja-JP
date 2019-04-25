---
title: internetMessageHeader リソースの種類
description: 'RFC5322 で定義されているように、インターネットメッセージヘッダーを表すキーと値のペア。 '
localization_priority: Normal
ms.openlocfilehash: 2a8dd616ffe8417a5064c0a98976d512b1279704
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567516"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="8ec25-103">internetMessageHeader リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ec25-103">internetMessageHeader resource type</span></span>


<span data-ttu-id="8ec25-104">[RFC5322](https://www.ietf.org/rfc/rfc5322.txt) によって定義された、インターネット メッセージ ヘッダーを表すキーと値のペア。メッセージが送信者から受信者に到達するまでに辿ったネットワーク パスの詳細を説明します。</span><span class="sxs-lookup"><span data-stu-id="8ec25-104">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="8ec25-105">インターネット メッセージ ヘッダーの例については、「[View e-mail message headers (電子メールのメッセージ ヘッダーを表示する)](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ec25-105">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="8ec25-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ec25-106">Properties</span></span>
| <span data-ttu-id="8ec25-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ec25-107">Property</span></span>     | <span data-ttu-id="8ec25-108">型</span><span class="sxs-lookup"><span data-stu-id="8ec25-108">Type</span></span>   |<span data-ttu-id="8ec25-109">説明</span><span class="sxs-lookup"><span data-stu-id="8ec25-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ec25-110">name</span><span class="sxs-lookup"><span data-stu-id="8ec25-110">name</span></span>|<span data-ttu-id="8ec25-111">string</span><span class="sxs-lookup"><span data-stu-id="8ec25-111">string</span></span>|<span data-ttu-id="8ec25-112">キーと値のペアの、キーの部分を表します。</span><span class="sxs-lookup"><span data-stu-id="8ec25-112">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="8ec25-113">value</span><span class="sxs-lookup"><span data-stu-id="8ec25-113">value</span></span>|<span data-ttu-id="8ec25-114">string</span><span class="sxs-lookup"><span data-stu-id="8ec25-114">string</span></span>|<span data-ttu-id="8ec25-115">キーと値のペアの、値の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="8ec25-115">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ec25-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ec25-116">JSON representation</span></span>

<span data-ttu-id="8ec25-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8ec25-117">Here is a JSON representation of the resource.</span></span>

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
