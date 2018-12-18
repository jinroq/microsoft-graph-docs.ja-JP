---
title: extendedKeyUsage リソースの種類
description: カスタムの拡張キー使用法の定義
author: tfitzmac
ms.openlocfilehash: 2b6155a0fbb234cb0b2081a8a4a226a8d218dbc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337290"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="c1a18-103">extendedKeyUsage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1a18-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="c1a18-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1a18-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1a18-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1a18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1a18-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1a18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1a18-107">カスタムの拡張キー使用法の定義</span><span class="sxs-lookup"><span data-stu-id="c1a18-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="c1a18-108">Properties</span><span class="sxs-lookup"><span data-stu-id="c1a18-108">Properties</span></span>
|<span data-ttu-id="c1a18-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1a18-109">Property</span></span>|<span data-ttu-id="c1a18-110">種類</span><span class="sxs-lookup"><span data-stu-id="c1a18-110">Type</span></span>|<span data-ttu-id="c1a18-111">説明</span><span class="sxs-lookup"><span data-stu-id="c1a18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1a18-112">名前</span><span class="sxs-lookup"><span data-stu-id="c1a18-112">name</span></span>|<span data-ttu-id="c1a18-113">String</span><span class="sxs-lookup"><span data-stu-id="c1a18-113">String</span></span>|<span data-ttu-id="c1a18-114">拡張キー使用法の名前</span><span class="sxs-lookup"><span data-stu-id="c1a18-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="c1a18-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="c1a18-115">objectIdentifier</span></span>|<span data-ttu-id="c1a18-116">String</span><span class="sxs-lookup"><span data-stu-id="c1a18-116">String</span></span>|<span data-ttu-id="c1a18-117">拡張キー使用法のオブジェクト識別子</span><span class="sxs-lookup"><span data-stu-id="c1a18-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1a18-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1a18-118">Relationships</span></span>
<span data-ttu-id="c1a18-119">なし</span><span class="sxs-lookup"><span data-stu-id="c1a18-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1a18-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1a18-120">JSON Representation</span></span>
<span data-ttu-id="c1a18-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1a18-121">Here is a JSON representation of the resource.</span></span>
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





