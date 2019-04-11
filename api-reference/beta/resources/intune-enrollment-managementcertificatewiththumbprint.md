---
title: managementcertificatewiththumbprint リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58b45f092848be7198141a34a443471426be273b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773708"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="8ec63-103">managementcertificatewiththumbprint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ec63-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="8ec63-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ec63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ec63-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ec63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ec63-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8ec63-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8ec63-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ec63-107">Properties</span></span>
|<span data-ttu-id="8ec63-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ec63-108">Property</span></span>|<span data-ttu-id="8ec63-109">型</span><span class="sxs-lookup"><span data-stu-id="8ec63-109">Type</span></span>|<span data-ttu-id="8ec63-110">説明</span><span class="sxs-lookup"><span data-stu-id="8ec63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ec63-111">拇印</span><span class="sxs-lookup"><span data-stu-id="8ec63-111">thumbprint</span></span>|<span data-ttu-id="8ec63-112">文字列</span><span class="sxs-lookup"><span data-stu-id="8ec63-112">String</span></span>|<span data-ttu-id="8ec63-113">管理証明書の拇印</span><span class="sxs-lookup"><span data-stu-id="8ec63-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="8ec63-114">certificate</span><span class="sxs-lookup"><span data-stu-id="8ec63-114">certificate</span></span>|<span data-ttu-id="8ec63-115">String</span><span class="sxs-lookup"><span data-stu-id="8ec63-115">String</span></span>|<span data-ttu-id="8ec63-116">Base 64 エンコード済み管理証明書</span><span class="sxs-lookup"><span data-stu-id="8ec63-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ec63-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8ec63-117">Relationships</span></span>
<span data-ttu-id="8ec63-118">なし</span><span class="sxs-lookup"><span data-stu-id="8ec63-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ec63-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ec63-119">JSON Representation</span></span>
<span data-ttu-id="8ec63-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8ec63-120">Here is a JSON representation of the resource.</span></span>
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





