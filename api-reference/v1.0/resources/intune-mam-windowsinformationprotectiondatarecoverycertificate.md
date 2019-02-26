---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c321ea06e27e7d6fba0a35446e2b916aaf0689de
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253653"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="dda76-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dda76-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="dda76-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dda76-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dda76-105">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="dda76-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="dda76-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dda76-106">Properties</span></span>
|<span data-ttu-id="dda76-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dda76-107">Property</span></span>|<span data-ttu-id="dda76-108">型</span><span class="sxs-lookup"><span data-stu-id="dda76-108">Type</span></span>|<span data-ttu-id="dda76-109">説明</span><span class="sxs-lookup"><span data-stu-id="dda76-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dda76-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="dda76-110">subjectName</span></span>|<span data-ttu-id="dda76-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dda76-111">String</span></span>|<span data-ttu-id="dda76-112">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="dda76-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="dda76-113">説明</span><span class="sxs-lookup"><span data-stu-id="dda76-113">description</span></span>|<span data-ttu-id="dda76-114">String</span><span class="sxs-lookup"><span data-stu-id="dda76-114">String</span></span>|<span data-ttu-id="dda76-115">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="dda76-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="dda76-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dda76-116">expirationDateTime</span></span>|<span data-ttu-id="dda76-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dda76-117">DateTimeOffset</span></span>|<span data-ttu-id="dda76-118">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="dda76-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="dda76-119">certificate</span><span class="sxs-lookup"><span data-stu-id="dda76-119">certificate</span></span>|<span data-ttu-id="dda76-120">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="dda76-120">Binary</span></span>|<span data-ttu-id="dda76-121">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="dda76-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="dda76-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dda76-122">Relationships</span></span>
<span data-ttu-id="dda76-123">なし</span><span class="sxs-lookup"><span data-stu-id="dda76-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dda76-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dda76-124">JSON Representation</span></span>
<span data-ttu-id="dda76-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dda76-125">Here is a JSON representation of the resource.</span></span>
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



