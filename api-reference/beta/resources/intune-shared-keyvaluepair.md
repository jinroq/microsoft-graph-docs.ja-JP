---
title: keyValuePair リソースの種類
description: カスタム設定の保存用のキーと値のペア
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9d7b5551bf4ca3237c6a4fc08db51c8e08474c63
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957901"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="3d5bb-103">keyValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d5bb-103">keyValuePair resource type</span></span>

> <span data-ttu-id="3d5bb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3d5bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d5bb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d5bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d5bb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d5bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d5bb-107">カスタム設定の保存用のキーと値のペア</span><span class="sxs-lookup"><span data-stu-id="3d5bb-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="3d5bb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d5bb-108">Properties</span></span>
|<span data-ttu-id="3d5bb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d5bb-109">Property</span></span>|<span data-ttu-id="3d5bb-110">型</span><span class="sxs-lookup"><span data-stu-id="3d5bb-110">Type</span></span>|<span data-ttu-id="3d5bb-111">説明</span><span class="sxs-lookup"><span data-stu-id="3d5bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d5bb-112">名前</span><span class="sxs-lookup"><span data-stu-id="3d5bb-112">name</span></span>|<span data-ttu-id="3d5bb-113">文字列</span><span class="sxs-lookup"><span data-stu-id="3d5bb-113">String</span></span>|<span data-ttu-id="3d5bb-114">キーと値のペアの名前</span><span class="sxs-lookup"><span data-stu-id="3d5bb-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="3d5bb-115">value</span><span class="sxs-lookup"><span data-stu-id="3d5bb-115">value</span></span>|<span data-ttu-id="3d5bb-116">文字列</span><span class="sxs-lookup"><span data-stu-id="3d5bb-116">String</span></span>|<span data-ttu-id="3d5bb-117">キーと値のペアの値</span><span class="sxs-lookup"><span data-stu-id="3d5bb-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d5bb-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3d5bb-118">Relationships</span></span>
<span data-ttu-id="3d5bb-119">なし</span><span class="sxs-lookup"><span data-stu-id="3d5bb-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3d5bb-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d5bb-120">JSON Representation</span></span>
<span data-ttu-id="3d5bb-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3d5bb-121">Here is a JSON representation of the resource.</span></span>
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





