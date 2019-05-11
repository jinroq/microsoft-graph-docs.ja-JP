---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dcdd83346072a6f2946060a68064989b44ca3eb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940604"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="11cb9-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="11cb9-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="11cb9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11cb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11cb9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="11cb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11cb9-106">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="11cb9-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="11cb9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11cb9-107">Properties</span></span>
|<span data-ttu-id="11cb9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11cb9-108">Property</span></span>|<span data-ttu-id="11cb9-109">型</span><span class="sxs-lookup"><span data-stu-id="11cb9-109">Type</span></span>|<span data-ttu-id="11cb9-110">説明</span><span class="sxs-lookup"><span data-stu-id="11cb9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11cb9-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="11cb9-111">subjectName</span></span>|<span data-ttu-id="11cb9-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="11cb9-112">String</span></span>|<span data-ttu-id="11cb9-113">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="11cb9-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="11cb9-114">description</span><span class="sxs-lookup"><span data-stu-id="11cb9-114">description</span></span>|<span data-ttu-id="11cb9-115">String</span><span class="sxs-lookup"><span data-stu-id="11cb9-115">String</span></span>|<span data-ttu-id="11cb9-116">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="11cb9-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="11cb9-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="11cb9-117">expirationDateTime</span></span>|<span data-ttu-id="11cb9-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11cb9-118">DateTimeOffset</span></span>|<span data-ttu-id="11cb9-119">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="11cb9-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="11cb9-120">certificate</span><span class="sxs-lookup"><span data-stu-id="11cb9-120">certificate</span></span>|<span data-ttu-id="11cb9-121">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="11cb9-121">Binary</span></span>|<span data-ttu-id="11cb9-122">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="11cb9-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="11cb9-123">関係</span><span class="sxs-lookup"><span data-stu-id="11cb9-123">Relationships</span></span>
<span data-ttu-id="11cb9-124">なし</span><span class="sxs-lookup"><span data-stu-id="11cb9-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11cb9-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="11cb9-125">JSON Representation</span></span>
<span data-ttu-id="11cb9-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="11cb9-126">Here is a JSON representation of the resource.</span></span>
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




