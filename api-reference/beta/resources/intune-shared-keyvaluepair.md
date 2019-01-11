---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 056dbe1f8504a89e3551402de7aa7ff7bc0ce866
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858444"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="3737d-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3737d-103">keyValuePair resource type</span></span>

> <span data-ttu-id="3737d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3737d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3737d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3737d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3737d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3737d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3737d-107">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="3737d-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="3737d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3737d-108">Properties</span></span>
|<span data-ttu-id="3737d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3737d-109">Property</span></span>|<span data-ttu-id="3737d-110">種類</span><span class="sxs-lookup"><span data-stu-id="3737d-110">Type</span></span>|<span data-ttu-id="3737d-111">説明</span><span class="sxs-lookup"><span data-stu-id="3737d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3737d-112">名前</span><span class="sxs-lookup"><span data-stu-id="3737d-112">name</span></span>|<span data-ttu-id="3737d-113">文字列</span><span class="sxs-lookup"><span data-stu-id="3737d-113">String</span></span>|<span data-ttu-id="3737d-114">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="3737d-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="3737d-115">value</span><span class="sxs-lookup"><span data-stu-id="3737d-115">value</span></span>|<span data-ttu-id="3737d-116">文字列</span><span class="sxs-lookup"><span data-stu-id="3737d-116">String</span></span>|<span data-ttu-id="3737d-117">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="3737d-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="3737d-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3737d-118">Relationships</span></span>
<span data-ttu-id="3737d-119">なし</span><span class="sxs-lookup"><span data-stu-id="3737d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3737d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3737d-120">JSON Representation</span></span>
<span data-ttu-id="3737d-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3737d-121">Here is a JSON representation of the resource.</span></span>
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





