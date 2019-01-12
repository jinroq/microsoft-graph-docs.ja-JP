---
title: extendedKeyUsage リソースの種類
description: カスタムの拡張キー使用法の定義
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bb08bf086ce8386e424ebd6355a4920e87be59a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928445"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="4a5a4-103">extendedKeyUsage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4a5a4-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="4a5a4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a5a4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a5a4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a5a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a5a4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a5a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a5a4-107">カスタムの拡張キー使用法の定義</span><span class="sxs-lookup"><span data-stu-id="4a5a4-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="4a5a4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a5a4-108">Properties</span></span>
|<span data-ttu-id="4a5a4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a5a4-109">Property</span></span>|<span data-ttu-id="4a5a4-110">種類</span><span class="sxs-lookup"><span data-stu-id="4a5a4-110">Type</span></span>|<span data-ttu-id="4a5a4-111">説明</span><span class="sxs-lookup"><span data-stu-id="4a5a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a5a4-112">名前</span><span class="sxs-lookup"><span data-stu-id="4a5a4-112">name</span></span>|<span data-ttu-id="4a5a4-113">String</span><span class="sxs-lookup"><span data-stu-id="4a5a4-113">String</span></span>|<span data-ttu-id="4a5a4-114">拡張キー使用法の名前</span><span class="sxs-lookup"><span data-stu-id="4a5a4-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="4a5a4-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="4a5a4-115">objectIdentifier</span></span>|<span data-ttu-id="4a5a4-116">String</span><span class="sxs-lookup"><span data-stu-id="4a5a4-116">String</span></span>|<span data-ttu-id="4a5a4-117">拡張キー使用法のオブジェクト識別子</span><span class="sxs-lookup"><span data-stu-id="4a5a4-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a5a4-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4a5a4-118">Relationships</span></span>
<span data-ttu-id="4a5a4-119">なし</span><span class="sxs-lookup"><span data-stu-id="4a5a4-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4a5a4-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4a5a4-120">JSON Representation</span></span>
<span data-ttu-id="4a5a4-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4a5a4-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```





