---
title: bitlockerrecoveryoptions リソースの種類
description: BitLocker 回復オプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5652add71ba19b1eba102a0579a787d7410d6c89
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791475"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="29372-103">bitlockerrecoveryoptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29372-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="29372-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29372-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29372-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29372-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29372-106">BitLocker 回復オプション。</span><span class="sxs-lookup"><span data-stu-id="29372-106">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="29372-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29372-107">Properties</span></span>
|<span data-ttu-id="29372-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29372-108">Property</span></span>|<span data-ttu-id="29372-109">型</span><span class="sxs-lookup"><span data-stu-id="29372-109">Type</span></span>|<span data-ttu-id="29372-110">説明</span><span class="sxs-lookup"><span data-stu-id="29372-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29372-111">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="29372-111">blockDataRecoveryAgent</span></span>|<span data-ttu-id="29372-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="29372-112">Boolean</span></span>|<span data-ttu-id="29372-113">証明書ベースのデータ回復エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29372-113">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="29372-114">回復した ypasswordusage</span><span class="sxs-lookup"><span data-stu-id="29372-114">recoveryPasswordUsage</span></span>|[<span data-ttu-id="29372-115">configurationusage</span><span class="sxs-lookup"><span data-stu-id="29372-115">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="29372-116">ユーザーが固定またはシステムディスク用に48桁の回復パスワードを生成することを許可または要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29372-116">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="29372-117">使用可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="29372-117">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="29372-118">recoverykeyusage</span><span class="sxs-lookup"><span data-stu-id="29372-118">recoveryKeyUsage</span></span>|[<span data-ttu-id="29372-119">configurationusage</span><span class="sxs-lookup"><span data-stu-id="29372-119">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="29372-120">ユーザーが固定またはシステムディスクの256ビット回復キーを生成することを許可または要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29372-120">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="29372-121">使用可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="29372-121">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="29372-122">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="29372-122">hideRecoveryOptions</span></span>|<span data-ttu-id="29372-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="29372-123">Boolean</span></span>|<span data-ttu-id="29372-124">固定またはシステムディスクの BitLocker セットアップウィザードでの復元オプションの表示を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29372-124">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="29372-125">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="29372-125">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="29372-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="29372-126">Boolean</span></span>|<span data-ttu-id="29372-127">AD DS に BitLocker 回復情報を格納することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29372-127">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="29372-128">recoveryinformationtostore</span><span class="sxs-lookup"><span data-stu-id="29372-128">recoveryInformationToStore</span></span>|[<span data-ttu-id="29372-129">bitLockerRecoveryinformationType</span><span class="sxs-lookup"><span data-stu-id="29372-129">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="29372-130">AD DS に格納される BitLocker 回復情報の種類を構成します。</span><span class="sxs-lookup"><span data-stu-id="29372-130">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="29372-131">可能な値は、`passwordAndKey`、`passwordOnly` です。</span><span class="sxs-lookup"><span data-stu-id="29372-131">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="29372-132">enablebitlockerafterrecoveryinformationtostore</span><span class="sxs-lookup"><span data-stu-id="29372-132">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="29372-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="29372-133">Boolean</span></span>|<span data-ttu-id="29372-134">AD DS に回復情報が格納されるまで BitLocker を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29372-134">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29372-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29372-135">Relationships</span></span>
<span data-ttu-id="29372-136">なし</span><span class="sxs-lookup"><span data-stu-id="29372-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29372-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29372-137">JSON Representation</span></span>
<span data-ttu-id="29372-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29372-138">Here is a JSON representation of the resource.</span></span>
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





