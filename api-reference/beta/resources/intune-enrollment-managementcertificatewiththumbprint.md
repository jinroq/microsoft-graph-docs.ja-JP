---
title: managementCertificateWithThumbprint リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d8f18e7fc117f00f99346267f544abc7d12db17e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827217"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="c6b48-103">managementCertificateWithThumbprint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c6b48-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="c6b48-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c6b48-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6b48-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6b48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6b48-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c6b48-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6b48-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c6b48-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c6b48-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6b48-108">Properties</span></span>
|<span data-ttu-id="c6b48-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6b48-109">Property</span></span>|<span data-ttu-id="c6b48-110">種類</span><span class="sxs-lookup"><span data-stu-id="c6b48-110">Type</span></span>|<span data-ttu-id="c6b48-111">説明</span><span class="sxs-lookup"><span data-stu-id="c6b48-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6b48-112">拇印</span><span class="sxs-lookup"><span data-stu-id="c6b48-112">thumbprint</span></span>|<span data-ttu-id="c6b48-113">String</span><span class="sxs-lookup"><span data-stu-id="c6b48-113">String</span></span>|<span data-ttu-id="c6b48-114">管理証明書の拇印</span><span class="sxs-lookup"><span data-stu-id="c6b48-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="c6b48-115">証明書</span><span class="sxs-lookup"><span data-stu-id="c6b48-115">certificate</span></span>|<span data-ttu-id="c6b48-116">String</span><span class="sxs-lookup"><span data-stu-id="c6b48-116">String</span></span>|<span data-ttu-id="c6b48-117">Base 64 にエンコードされた証明書の管理</span><span class="sxs-lookup"><span data-stu-id="c6b48-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6b48-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c6b48-118">Relationships</span></span>
<span data-ttu-id="c6b48-119">なし</span><span class="sxs-lookup"><span data-stu-id="c6b48-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6b48-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6b48-120">JSON Representation</span></span>
<span data-ttu-id="c6b48-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c6b48-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```





