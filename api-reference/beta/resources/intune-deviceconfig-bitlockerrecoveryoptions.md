---
title: bitLockerRecoveryOptions リソースの種類
description: BitLocker 回復オプション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf88795ac9f2708bc03607bc5d48d5ec69a822eb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991052"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="da1e1-103">bitLockerRecoveryOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="da1e1-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="da1e1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da1e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da1e1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da1e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da1e1-106">BitLocker 回復オプション。</span><span class="sxs-lookup"><span data-stu-id="da1e1-106">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="da1e1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da1e1-107">Properties</span></span>
|<span data-ttu-id="da1e1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da1e1-108">Property</span></span>|<span data-ttu-id="da1e1-109">型</span><span class="sxs-lookup"><span data-stu-id="da1e1-109">Type</span></span>|<span data-ttu-id="da1e1-110">説明</span><span class="sxs-lookup"><span data-stu-id="da1e1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da1e1-111">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="da1e1-111">blockDataRecoveryAgent</span></span>|<span data-ttu-id="da1e1-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="da1e1-112">Boolean</span></span>|<span data-ttu-id="da1e1-113">証明書ベースのデータ回復エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="da1e1-113">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="da1e1-114">回復した Ypasswordusage</span><span class="sxs-lookup"><span data-stu-id="da1e1-114">recoveryPasswordUsage</span></span>|[<span data-ttu-id="da1e1-115">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="da1e1-115">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="da1e1-116">ユーザーが固定またはシステムディスク用に48桁の回復パスワードを生成することを許可または要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="da1e1-116">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="da1e1-117">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="da1e1-117">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="da1e1-118">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="da1e1-118">recoveryKeyUsage</span></span>|[<span data-ttu-id="da1e1-119">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="da1e1-119">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="da1e1-120">ユーザーが固定またはシステムディスクの256ビット回復キーを生成することを許可または要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="da1e1-120">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="da1e1-121">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="da1e1-121">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="da1e1-122">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="da1e1-122">hideRecoveryOptions</span></span>|<span data-ttu-id="da1e1-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="da1e1-123">Boolean</span></span>|<span data-ttu-id="da1e1-124">固定またはシステムディスクの BitLocker セットアップウィザードでの復元オプションの表示を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="da1e1-124">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="da1e1-125">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="da1e1-125">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="da1e1-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="da1e1-126">Boolean</span></span>|<span data-ttu-id="da1e1-127">AD DS に BitLocker 回復情報を格納することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="da1e1-127">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="da1e1-128">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="da1e1-128">recoveryInformationToStore</span></span>|[<span data-ttu-id="da1e1-129">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="da1e1-129">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="da1e1-130">AD DS に格納される BitLocker 回復情報の種類を構成します。</span><span class="sxs-lookup"><span data-stu-id="da1e1-130">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="da1e1-131">可能な値は、`passwordAndKey`、`passwordOnly` です。</span><span class="sxs-lookup"><span data-stu-id="da1e1-131">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="da1e1-132">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="da1e1-132">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="da1e1-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="da1e1-133">Boolean</span></span>|<span data-ttu-id="da1e1-134">AD DS に回復情報が格納されるまで BitLocker を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="da1e1-134">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da1e1-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da1e1-135">Relationships</span></span>
<span data-ttu-id="da1e1-136">なし</span><span class="sxs-lookup"><span data-stu-id="da1e1-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da1e1-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da1e1-137">JSON Representation</span></span>
<span data-ttu-id="da1e1-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="da1e1-138">Here is a JSON representation of the resource.</span></span>
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





