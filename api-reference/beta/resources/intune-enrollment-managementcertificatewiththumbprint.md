---
title: managementCertificateWithThumbprint リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 320b6241e1ac5a9078ccc32f99f87e9fd337335e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071310"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="571a3-103">managementCertificateWithThumbprint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="571a3-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="571a3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="571a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="571a3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="571a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="571a3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="571a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="571a3-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="571a3-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="571a3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="571a3-108">Properties</span></span>
|<span data-ttu-id="571a3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="571a3-109">Property</span></span>|<span data-ttu-id="571a3-110">型</span><span class="sxs-lookup"><span data-stu-id="571a3-110">Type</span></span>|<span data-ttu-id="571a3-111">説明</span><span class="sxs-lookup"><span data-stu-id="571a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="571a3-112">拇印</span><span class="sxs-lookup"><span data-stu-id="571a3-112">thumbprint</span></span>|<span data-ttu-id="571a3-113">String</span><span class="sxs-lookup"><span data-stu-id="571a3-113">String</span></span>|<span data-ttu-id="571a3-114">管理証明書の拇印</span><span class="sxs-lookup"><span data-stu-id="571a3-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="571a3-115">証明書</span><span class="sxs-lookup"><span data-stu-id="571a3-115">certificate</span></span>|<span data-ttu-id="571a3-116">String</span><span class="sxs-lookup"><span data-stu-id="571a3-116">String</span></span>|<span data-ttu-id="571a3-117">Base 64 にエンコードされた証明書の管理</span><span class="sxs-lookup"><span data-stu-id="571a3-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="571a3-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="571a3-118">Relationships</span></span>
<span data-ttu-id="571a3-119">なし</span><span class="sxs-lookup"><span data-stu-id="571a3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="571a3-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="571a3-120">JSON Representation</span></span>
<span data-ttu-id="571a3-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="571a3-121">Here is a JSON representation of the resource.</span></span>
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





