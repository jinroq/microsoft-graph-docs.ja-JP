---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 555cac098d2796f612054f11e2c5ade525ad6199
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037731"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="0273e-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0273e-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="0273e-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0273e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0273e-105">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="0273e-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="0273e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0273e-106">Properties</span></span>
|<span data-ttu-id="0273e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0273e-107">Property</span></span>|<span data-ttu-id="0273e-108">型</span><span class="sxs-lookup"><span data-stu-id="0273e-108">Type</span></span>|<span data-ttu-id="0273e-109">説明</span><span class="sxs-lookup"><span data-stu-id="0273e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0273e-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="0273e-110">subjectName</span></span>|<span data-ttu-id="0273e-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0273e-111">String</span></span>|<span data-ttu-id="0273e-112">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="0273e-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="0273e-113">description</span><span class="sxs-lookup"><span data-stu-id="0273e-113">description</span></span>|<span data-ttu-id="0273e-114">String</span><span class="sxs-lookup"><span data-stu-id="0273e-114">String</span></span>|<span data-ttu-id="0273e-115">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="0273e-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="0273e-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0273e-116">expirationDateTime</span></span>|<span data-ttu-id="0273e-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0273e-117">DateTimeOffset</span></span>|<span data-ttu-id="0273e-118">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="0273e-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="0273e-119">certificate</span><span class="sxs-lookup"><span data-stu-id="0273e-119">certificate</span></span>|<span data-ttu-id="0273e-120">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="0273e-120">Binary</span></span>|<span data-ttu-id="0273e-121">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="0273e-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="0273e-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0273e-122">Relationships</span></span>
<span data-ttu-id="0273e-123">なし</span><span class="sxs-lookup"><span data-stu-id="0273e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0273e-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0273e-124">JSON Representation</span></span>
<span data-ttu-id="0273e-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0273e-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



