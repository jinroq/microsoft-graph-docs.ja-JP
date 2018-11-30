---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
ms.openlocfilehash: 803dd9e347ef06bc9d4a9fce13d2265c4fc969a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023388"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="f1455-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1455-103">keyValuePair resource type</span></span>

> <span data-ttu-id="f1455-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1455-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1455-105">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="f1455-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="f1455-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1455-106">Properties</span></span>
|<span data-ttu-id="f1455-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1455-107">Property</span></span>|<span data-ttu-id="f1455-108">型</span><span class="sxs-lookup"><span data-stu-id="f1455-108">Type</span></span>|<span data-ttu-id="f1455-109">説明</span><span class="sxs-lookup"><span data-stu-id="f1455-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1455-110">名前</span><span class="sxs-lookup"><span data-stu-id="f1455-110">name</span></span>|<span data-ttu-id="f1455-111">文字列</span><span class="sxs-lookup"><span data-stu-id="f1455-111">String</span></span>|<span data-ttu-id="f1455-112">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="f1455-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="f1455-113">value</span><span class="sxs-lookup"><span data-stu-id="f1455-113">value</span></span>|<span data-ttu-id="f1455-114">文字列</span><span class="sxs-lookup"><span data-stu-id="f1455-114">String</span></span>|<span data-ttu-id="f1455-115">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="f1455-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1455-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f1455-116">Relationships</span></span>
<span data-ttu-id="f1455-117">なし</span><span class="sxs-lookup"><span data-stu-id="f1455-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1455-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1455-118">JSON Representation</span></span>
<span data-ttu-id="f1455-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f1455-119">Here is a JSON representation of the resource.</span></span>
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



