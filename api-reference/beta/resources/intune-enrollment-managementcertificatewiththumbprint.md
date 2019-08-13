---
title: managementCertificateWithThumbprint リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9fc6535147b8e7a5f2a2295b09cb73cce86c1793
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327809"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="da68a-103">managementCertificateWithThumbprint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="da68a-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="da68a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da68a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da68a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da68a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da68a-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="da68a-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="da68a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da68a-107">Properties</span></span>
|<span data-ttu-id="da68a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da68a-108">Property</span></span>|<span data-ttu-id="da68a-109">型</span><span class="sxs-lookup"><span data-stu-id="da68a-109">Type</span></span>|<span data-ttu-id="da68a-110">説明</span><span class="sxs-lookup"><span data-stu-id="da68a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da68a-111">拇印</span><span class="sxs-lookup"><span data-stu-id="da68a-111">thumbprint</span></span>|<span data-ttu-id="da68a-112">String</span><span class="sxs-lookup"><span data-stu-id="da68a-112">String</span></span>|<span data-ttu-id="da68a-113">管理証明書の拇印</span><span class="sxs-lookup"><span data-stu-id="da68a-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="da68a-114">certificate</span><span class="sxs-lookup"><span data-stu-id="da68a-114">certificate</span></span>|<span data-ttu-id="da68a-115">String</span><span class="sxs-lookup"><span data-stu-id="da68a-115">String</span></span>|<span data-ttu-id="da68a-116">Base 64 エンコード済み管理証明書</span><span class="sxs-lookup"><span data-stu-id="da68a-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="da68a-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da68a-117">Relationships</span></span>
<span data-ttu-id="da68a-118">なし</span><span class="sxs-lookup"><span data-stu-id="da68a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da68a-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da68a-119">JSON Representation</span></span>
<span data-ttu-id="da68a-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="da68a-120">Here is a JSON representation of the resource.</span></span>
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



