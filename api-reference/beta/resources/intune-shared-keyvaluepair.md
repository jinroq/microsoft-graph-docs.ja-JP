---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: tfitzmac
ms.openlocfilehash: f6438d97376d46f66e02026acc87c948ab2a91bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329317"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="6049a-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6049a-103">keyValuePair resource type</span></span>

> <span data-ttu-id="6049a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6049a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6049a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6049a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6049a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6049a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6049a-107">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="6049a-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="6049a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6049a-108">Properties</span></span>
|<span data-ttu-id="6049a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6049a-109">Property</span></span>|<span data-ttu-id="6049a-110">種類</span><span class="sxs-lookup"><span data-stu-id="6049a-110">Type</span></span>|<span data-ttu-id="6049a-111">説明</span><span class="sxs-lookup"><span data-stu-id="6049a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6049a-112">名前</span><span class="sxs-lookup"><span data-stu-id="6049a-112">name</span></span>|<span data-ttu-id="6049a-113">文字列</span><span class="sxs-lookup"><span data-stu-id="6049a-113">String</span></span>|<span data-ttu-id="6049a-114">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="6049a-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="6049a-115">value</span><span class="sxs-lookup"><span data-stu-id="6049a-115">value</span></span>|<span data-ttu-id="6049a-116">文字列</span><span class="sxs-lookup"><span data-stu-id="6049a-116">String</span></span>|<span data-ttu-id="6049a-117">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="6049a-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="6049a-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6049a-118">Relationships</span></span>
<span data-ttu-id="6049a-119">なし</span><span class="sxs-lookup"><span data-stu-id="6049a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6049a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6049a-120">JSON Representation</span></span>
<span data-ttu-id="6049a-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6049a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```





