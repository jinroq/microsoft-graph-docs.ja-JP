---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
ms.openlocfilehash: cc0d024c814588479e641114ad33d19a5e609ecd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072194"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="909ab-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="909ab-103">mimeContent resource type</span></span>

> <span data-ttu-id="909ab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="909ab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="909ab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="909ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="909ab-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="909ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="909ab-107">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="909ab-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="909ab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="909ab-108">Properties</span></span>
|<span data-ttu-id="909ab-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="909ab-109">Property</span></span>|<span data-ttu-id="909ab-110">型</span><span class="sxs-lookup"><span data-stu-id="909ab-110">Type</span></span>|<span data-ttu-id="909ab-111">説明</span><span class="sxs-lookup"><span data-stu-id="909ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="909ab-112">type</span><span class="sxs-lookup"><span data-stu-id="909ab-112">type</span></span>|<span data-ttu-id="909ab-113">String</span><span class="sxs-lookup"><span data-stu-id="909ab-113">String</span></span>|<span data-ttu-id="909ab-114">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="909ab-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="909ab-115">value</span><span class="sxs-lookup"><span data-stu-id="909ab-115">value</span></span>|<span data-ttu-id="909ab-116">バイナリ</span><span class="sxs-lookup"><span data-stu-id="909ab-116">Binary</span></span>|<span data-ttu-id="909ab-117">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="909ab-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="909ab-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="909ab-118">Relationships</span></span>
<span data-ttu-id="909ab-119">なし</span><span class="sxs-lookup"><span data-stu-id="909ab-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="909ab-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="909ab-120">JSON Representation</span></span>
<span data-ttu-id="909ab-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="909ab-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```





