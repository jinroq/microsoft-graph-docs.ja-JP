---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 44f1765fb4f03a287665fe4ed1faef7012a43459
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805895"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="805b9-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="805b9-103">keyValuePair resource type</span></span>

> <span data-ttu-id="805b9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="805b9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="805b9-105">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="805b9-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="805b9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="805b9-106">Properties</span></span>
|<span data-ttu-id="805b9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="805b9-107">Property</span></span>|<span data-ttu-id="805b9-108">種類</span><span class="sxs-lookup"><span data-stu-id="805b9-108">Type</span></span>|<span data-ttu-id="805b9-109">説明</span><span class="sxs-lookup"><span data-stu-id="805b9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="805b9-110">名前</span><span class="sxs-lookup"><span data-stu-id="805b9-110">name</span></span>|<span data-ttu-id="805b9-111">文字列</span><span class="sxs-lookup"><span data-stu-id="805b9-111">String</span></span>|<span data-ttu-id="805b9-112">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="805b9-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="805b9-113">value</span><span class="sxs-lookup"><span data-stu-id="805b9-113">value</span></span>|<span data-ttu-id="805b9-114">文字列</span><span class="sxs-lookup"><span data-stu-id="805b9-114">String</span></span>|<span data-ttu-id="805b9-115">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="805b9-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="805b9-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="805b9-116">Relationships</span></span>
<span data-ttu-id="805b9-117">なし</span><span class="sxs-lookup"><span data-stu-id="805b9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="805b9-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="805b9-118">JSON Representation</span></span>
<span data-ttu-id="805b9-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="805b9-119">Here is a JSON representation of the resource.</span></span>
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



