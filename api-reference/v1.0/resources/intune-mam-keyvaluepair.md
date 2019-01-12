---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db3e24c1c14cb208be66b7a2b0364ad12b162956
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926443"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="ef19d-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef19d-103">keyValuePair resource type</span></span>

> <span data-ttu-id="ef19d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef19d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef19d-105">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="ef19d-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="ef19d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef19d-106">Properties</span></span>
|<span data-ttu-id="ef19d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef19d-107">Property</span></span>|<span data-ttu-id="ef19d-108">種類</span><span class="sxs-lookup"><span data-stu-id="ef19d-108">Type</span></span>|<span data-ttu-id="ef19d-109">説明</span><span class="sxs-lookup"><span data-stu-id="ef19d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef19d-110">名前</span><span class="sxs-lookup"><span data-stu-id="ef19d-110">name</span></span>|<span data-ttu-id="ef19d-111">文字列</span><span class="sxs-lookup"><span data-stu-id="ef19d-111">String</span></span>|<span data-ttu-id="ef19d-112">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="ef19d-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="ef19d-113">value</span><span class="sxs-lookup"><span data-stu-id="ef19d-113">value</span></span>|<span data-ttu-id="ef19d-114">文字列</span><span class="sxs-lookup"><span data-stu-id="ef19d-114">String</span></span>|<span data-ttu-id="ef19d-115">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="ef19d-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef19d-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef19d-116">Relationships</span></span>
<span data-ttu-id="ef19d-117">なし</span><span class="sxs-lookup"><span data-stu-id="ef19d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ef19d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef19d-118">JSON Representation</span></span>
<span data-ttu-id="ef19d-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ef19d-119">Here is a JSON representation of the resource.</span></span>
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



