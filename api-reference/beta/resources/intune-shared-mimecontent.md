---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ee38eee9100982f6dc5f22315af480a783cc4252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962122"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="9cc64-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9cc64-103">mimeContent resource type</span></span>

> <span data-ttu-id="9cc64-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9cc64-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9cc64-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cc64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cc64-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9cc64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9cc64-107">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9cc64-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="9cc64-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9cc64-108">Properties</span></span>
|<span data-ttu-id="9cc64-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9cc64-109">Property</span></span>|<span data-ttu-id="9cc64-110">種類</span><span class="sxs-lookup"><span data-stu-id="9cc64-110">Type</span></span>|<span data-ttu-id="9cc64-111">説明</span><span class="sxs-lookup"><span data-stu-id="9cc64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cc64-112">type</span><span class="sxs-lookup"><span data-stu-id="9cc64-112">type</span></span>|<span data-ttu-id="9cc64-113">String</span><span class="sxs-lookup"><span data-stu-id="9cc64-113">String</span></span>|<span data-ttu-id="9cc64-114">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="9cc64-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="9cc64-115">value</span><span class="sxs-lookup"><span data-stu-id="9cc64-115">value</span></span>|<span data-ttu-id="9cc64-116">バイナリ</span><span class="sxs-lookup"><span data-stu-id="9cc64-116">Binary</span></span>|<span data-ttu-id="9cc64-117">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="9cc64-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cc64-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9cc64-118">Relationships</span></span>
<span data-ttu-id="9cc64-119">なし</span><span class="sxs-lookup"><span data-stu-id="9cc64-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9cc64-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9cc64-120">JSON Representation</span></span>
<span data-ttu-id="9cc64-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9cc64-121">Here is a JSON representation of the resource.</span></span>
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





