---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74c480b8117f3d8dbf0ad8208bac09b63b113906
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156190"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="795e8-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="795e8-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="795e8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="795e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="795e8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="795e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="795e8-106">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="795e8-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="795e8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="795e8-107">Properties</span></span>
|<span data-ttu-id="795e8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="795e8-108">Property</span></span>|<span data-ttu-id="795e8-109">型</span><span class="sxs-lookup"><span data-stu-id="795e8-109">Type</span></span>|<span data-ttu-id="795e8-110">説明</span><span class="sxs-lookup"><span data-stu-id="795e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="795e8-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="795e8-111">subjectName</span></span>|<span data-ttu-id="795e8-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="795e8-112">String</span></span>|<span data-ttu-id="795e8-113">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="795e8-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="795e8-114">説明</span><span class="sxs-lookup"><span data-stu-id="795e8-114">description</span></span>|<span data-ttu-id="795e8-115">String</span><span class="sxs-lookup"><span data-stu-id="795e8-115">String</span></span>|<span data-ttu-id="795e8-116">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="795e8-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="795e8-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="795e8-117">expirationDateTime</span></span>|<span data-ttu-id="795e8-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="795e8-118">DateTimeOffset</span></span>|<span data-ttu-id="795e8-119">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="795e8-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="795e8-120">certificate</span><span class="sxs-lookup"><span data-stu-id="795e8-120">certificate</span></span>|<span data-ttu-id="795e8-121">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="795e8-121">Binary</span></span>|<span data-ttu-id="795e8-122">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="795e8-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="795e8-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="795e8-123">Relationships</span></span>
<span data-ttu-id="795e8-124">なし</span><span class="sxs-lookup"><span data-stu-id="795e8-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="795e8-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="795e8-125">JSON Representation</span></span>
<span data-ttu-id="795e8-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="795e8-126">Here is a JSON representation of the resource.</span></span>
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




