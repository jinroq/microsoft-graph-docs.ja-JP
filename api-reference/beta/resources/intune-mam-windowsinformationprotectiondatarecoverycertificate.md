---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32a18b25209301e3aeb62aaeaf63f080955cf669
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994532"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="6a7a1-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a7a1-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="6a7a1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a7a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a7a1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a7a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a7a1-106">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="6a7a1-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="6a7a1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a7a1-107">Properties</span></span>
|<span data-ttu-id="6a7a1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a7a1-108">Property</span></span>|<span data-ttu-id="6a7a1-109">型</span><span class="sxs-lookup"><span data-stu-id="6a7a1-109">Type</span></span>|<span data-ttu-id="6a7a1-110">説明</span><span class="sxs-lookup"><span data-stu-id="6a7a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a7a1-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="6a7a1-111">subjectName</span></span>|<span data-ttu-id="6a7a1-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6a7a1-112">String</span></span>|<span data-ttu-id="6a7a1-113">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="6a7a1-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="6a7a1-114">description</span><span class="sxs-lookup"><span data-stu-id="6a7a1-114">description</span></span>|<span data-ttu-id="6a7a1-115">String</span><span class="sxs-lookup"><span data-stu-id="6a7a1-115">String</span></span>|<span data-ttu-id="6a7a1-116">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="6a7a1-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="6a7a1-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6a7a1-117">expirationDateTime</span></span>|<span data-ttu-id="6a7a1-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a7a1-118">DateTimeOffset</span></span>|<span data-ttu-id="6a7a1-119">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="6a7a1-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="6a7a1-120">certificate</span><span class="sxs-lookup"><span data-stu-id="6a7a1-120">certificate</span></span>|<span data-ttu-id="6a7a1-121">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="6a7a1-121">Binary</span></span>|<span data-ttu-id="6a7a1-122">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="6a7a1-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a7a1-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a7a1-123">Relationships</span></span>
<span data-ttu-id="6a7a1-124">なし</span><span class="sxs-lookup"><span data-stu-id="6a7a1-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a7a1-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a7a1-125">JSON Representation</span></span>
<span data-ttu-id="6a7a1-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a7a1-126">Here is a JSON representation of the resource.</span></span>
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





