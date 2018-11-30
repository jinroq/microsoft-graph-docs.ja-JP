---
title: extendedKeyUsage リソースの種類
description: カスタムの拡張キー使用法の定義
ms.openlocfilehash: bbf869dd32c384a12aa8e80e8a3b5984e699de48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066530"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="5b0ea-103">extendedKeyUsage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b0ea-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="5b0ea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b0ea-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b0ea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b0ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b0ea-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b0ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b0ea-107">カスタムの拡張キー使用法の定義</span><span class="sxs-lookup"><span data-stu-id="5b0ea-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="5b0ea-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b0ea-108">Properties</span></span>
|<span data-ttu-id="5b0ea-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b0ea-109">Property</span></span>|<span data-ttu-id="5b0ea-110">型</span><span class="sxs-lookup"><span data-stu-id="5b0ea-110">Type</span></span>|<span data-ttu-id="5b0ea-111">説明</span><span class="sxs-lookup"><span data-stu-id="5b0ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b0ea-112">名前</span><span class="sxs-lookup"><span data-stu-id="5b0ea-112">name</span></span>|<span data-ttu-id="5b0ea-113">String</span><span class="sxs-lookup"><span data-stu-id="5b0ea-113">String</span></span>|<span data-ttu-id="5b0ea-114">拡張キー使用法の名前</span><span class="sxs-lookup"><span data-stu-id="5b0ea-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="5b0ea-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="5b0ea-115">objectIdentifier</span></span>|<span data-ttu-id="5b0ea-116">String</span><span class="sxs-lookup"><span data-stu-id="5b0ea-116">String</span></span>|<span data-ttu-id="5b0ea-117">拡張キー使用法のオブジェクト識別子</span><span class="sxs-lookup"><span data-stu-id="5b0ea-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b0ea-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5b0ea-118">Relationships</span></span>
<span data-ttu-id="5b0ea-119">なし</span><span class="sxs-lookup"><span data-stu-id="5b0ea-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b0ea-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b0ea-120">JSON Representation</span></span>
<span data-ttu-id="5b0ea-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5b0ea-121">Here is a JSON representation of the resource.</span></span>
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





