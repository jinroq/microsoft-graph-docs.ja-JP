---
title: managementcertificatewiththumbprint リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58b45f092848be7198141a34a443471426be273b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547166"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="ea425-103">managementcertificatewiththumbprint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ea425-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="ea425-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea425-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea425-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ea425-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea425-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ea425-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ea425-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea425-107">Properties</span></span>
|<span data-ttu-id="ea425-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea425-108">Property</span></span>|<span data-ttu-id="ea425-109">型</span><span class="sxs-lookup"><span data-stu-id="ea425-109">Type</span></span>|<span data-ttu-id="ea425-110">説明</span><span class="sxs-lookup"><span data-stu-id="ea425-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea425-111">拇印</span><span class="sxs-lookup"><span data-stu-id="ea425-111">thumbprint</span></span>|<span data-ttu-id="ea425-112">String</span><span class="sxs-lookup"><span data-stu-id="ea425-112">String</span></span>|<span data-ttu-id="ea425-113">管理証明書の拇印</span><span class="sxs-lookup"><span data-stu-id="ea425-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="ea425-114">certificate</span><span class="sxs-lookup"><span data-stu-id="ea425-114">certificate</span></span>|<span data-ttu-id="ea425-115">String</span><span class="sxs-lookup"><span data-stu-id="ea425-115">String</span></span>|<span data-ttu-id="ea425-116">Base 64 エンコード済み管理証明書</span><span class="sxs-lookup"><span data-stu-id="ea425-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea425-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ea425-117">Relationships</span></span>
<span data-ttu-id="ea425-118">なし</span><span class="sxs-lookup"><span data-stu-id="ea425-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea425-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ea425-119">JSON Representation</span></span>
<span data-ttu-id="ea425-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ea425-120">Here is a JSON representation of the resource.</span></span>
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





