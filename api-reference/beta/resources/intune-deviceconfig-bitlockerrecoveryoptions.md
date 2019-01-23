---
title: bitLockerRecoveryOptions リソースの種類
description: BitLocker の回復オプションです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df1a2d0a9be3f4ec52b5fa289d0315bda36e4a59
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398514"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="8cc51-103">bitLockerRecoveryOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cc51-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="8cc51-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8cc51-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8cc51-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cc51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8cc51-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cc51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc51-107">BitLocker の回復オプションです。</span><span class="sxs-lookup"><span data-stu-id="8cc51-107">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="8cc51-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cc51-108">Properties</span></span>
|<span data-ttu-id="8cc51-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cc51-109">Property</span></span>|<span data-ttu-id="8cc51-110">型</span><span class="sxs-lookup"><span data-stu-id="8cc51-110">Type</span></span>|<span data-ttu-id="8cc51-111">説明</span><span class="sxs-lookup"><span data-stu-id="8cc51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc51-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="8cc51-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="8cc51-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc51-113">Boolean</span></span>|<span data-ttu-id="8cc51-114">回復エージェントの証明書ベースのデータをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8cc51-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="8cc51-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="8cc51-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="8cc51-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="8cc51-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="8cc51-117">ユーザーの許可または固定の 48 桁の回復パスワードを生成するために必要なのかどうか、またはシステム ディスクを示します。</span><span class="sxs-lookup"><span data-stu-id="8cc51-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="8cc51-118">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="8cc51-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="8cc51-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="8cc51-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="8cc51-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="8cc51-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="8cc51-121">ユーザーの許可または固定の 256 ビットの回復キーを生成するために必要なのかどうか、またはシステム ディスクを示します。</span><span class="sxs-lookup"><span data-stu-id="8cc51-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="8cc51-122">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="8cc51-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="8cc51-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="8cc51-123">hideRecoveryOptions</span></span>|<span data-ttu-id="8cc51-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc51-124">Boolean</span></span>|<span data-ttu-id="8cc51-125">固定の BitLocker セットアップ ウィザードの回復オプションを表示できるようにするかどうか、またはシステム ディスクを示します。</span><span class="sxs-lookup"><span data-stu-id="8cc51-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="8cc51-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="8cc51-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="8cc51-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc51-127">Boolean</span></span>|<span data-ttu-id="8cc51-128">AD DS に格納するのには BitLocker 回復情報を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8cc51-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="8cc51-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="8cc51-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="8cc51-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="8cc51-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="8cc51-131">どのようなさまざまな BitLocker 回復情報が AD DS に格納されている構成です。</span><span class="sxs-lookup"><span data-stu-id="8cc51-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="8cc51-132">使用可能な値は、`passwordAndKey`、`passwordOnly` です。</span><span class="sxs-lookup"><span data-stu-id="8cc51-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="8cc51-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="8cc51-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="8cc51-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc51-134">Boolean</span></span>|<span data-ttu-id="8cc51-135">AD DS に回復情報が格納されるまで BitLocker を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8cc51-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cc51-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8cc51-136">Relationships</span></span>
<span data-ttu-id="8cc51-137">なし</span><span class="sxs-lookup"><span data-stu-id="8cc51-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cc51-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cc51-138">JSON Representation</span></span>
<span data-ttu-id="8cc51-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8cc51-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```




