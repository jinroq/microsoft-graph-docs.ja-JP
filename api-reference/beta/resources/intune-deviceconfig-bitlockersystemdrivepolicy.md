---
title: bitLockerSystemDrivePolicy リソースの種類
description: BitLocker 暗号化の基本ポリシーです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b63d075538508941d012df1e44f7cb563fed20d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425709"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="889e9-103">bitLockerSystemDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="889e9-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="889e9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="889e9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="889e9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="889e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="889e9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="889e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="889e9-107">BitLocker 暗号化の基本ポリシーです。</span><span class="sxs-lookup"><span data-stu-id="889e9-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="889e9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="889e9-108">Properties</span></span>
|<span data-ttu-id="889e9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="889e9-109">Property</span></span>|<span data-ttu-id="889e9-110">型</span><span class="sxs-lookup"><span data-stu-id="889e9-110">Type</span></span>|<span data-ttu-id="889e9-111">説明</span><span class="sxs-lookup"><span data-stu-id="889e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="889e9-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="889e9-112">encryptionMethod</span></span>|[<span data-ttu-id="889e9-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="889e9-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="889e9-114">オペレーティング システム ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="889e9-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="889e9-115">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="889e9-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="889e9-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="889e9-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="889e9-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="889e9-117">Boolean</span></span>|<span data-ttu-id="889e9-118">起動時に追加の認証が必要です。</span><span class="sxs-lookup"><span data-stu-id="889e9-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="889e9-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="889e9-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="889e9-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="889e9-120">Boolean</span></span>|<span data-ttu-id="889e9-121">なし (または USB フラッシュ ドライブにスタートアップ キーのパスワードが必要です)、互換性のある TPM は BitLocker を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="889e9-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="889e9-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="889e9-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="889e9-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="889e9-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="889e9-124">TPM スタートアップを許可または必要と許可しないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="889e9-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="889e9-125">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="889e9-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="889e9-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="889e9-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="889e9-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="889e9-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="889e9-128">TPM スタートアップの暗証番号 (pin) を許可または必要と許可しないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="889e9-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="889e9-129">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="889e9-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="889e9-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="889e9-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="889e9-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="889e9-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="889e9-132">スタートアップ キーを TPM を許可または必要と許可しないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="889e9-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="889e9-133">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="889e9-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="889e9-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="889e9-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="889e9-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="889e9-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="889e9-136">TPM スタートアップに追加することを示しますキーとキーは、許可または必要と許可しません。</span><span class="sxs-lookup"><span data-stu-id="889e9-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="889e9-137">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="889e9-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="889e9-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="889e9-138">minimumPinLength</span></span>|<span data-ttu-id="889e9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="889e9-139">Int32</span></span>|<span data-ttu-id="889e9-140">スタートアップの暗証番号 (pin) の最小の長さを示します。</span><span class="sxs-lookup"><span data-stu-id="889e9-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="889e9-141">4 ~ 20 の有効な値</span><span class="sxs-lookup"><span data-stu-id="889e9-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="889e9-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="889e9-142">recoveryOptions</span></span>|[<span data-ttu-id="889e9-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="889e9-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="889e9-144">必要なスタートアップ キー情報がない場合、BitLocker で暗号化されたオペレーティング システム ドライブを回復することができます。</span><span class="sxs-lookup"><span data-stu-id="889e9-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="889e9-145">BitLocker を有効にするときは、このポリシー設定が適用されます。</span><span class="sxs-lookup"><span data-stu-id="889e9-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="889e9-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="889e9-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="889e9-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="889e9-147">Boolean</span></span>|<span data-ttu-id="889e9-148">ブート前の回復のメッセージと Url を有効にします。</span><span class="sxs-lookup"><span data-stu-id="889e9-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="889e9-149">RequireStartupAuthentication が false の場合、この値は影響しません。</span><span class="sxs-lookup"><span data-stu-id="889e9-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="889e9-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="889e9-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="889e9-151">String</span><span class="sxs-lookup"><span data-stu-id="889e9-151">String</span></span>|<span data-ttu-id="889e9-152">回復のカスタム メッセージを定義します。</span><span class="sxs-lookup"><span data-stu-id="889e9-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="889e9-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="889e9-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="889e9-154">String</span><span class="sxs-lookup"><span data-stu-id="889e9-154">String</span></span>|<span data-ttu-id="889e9-155">回復のカスタム URL を定義します。</span><span class="sxs-lookup"><span data-stu-id="889e9-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="889e9-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="889e9-156">Relationships</span></span>
<span data-ttu-id="889e9-157">なし</span><span class="sxs-lookup"><span data-stu-id="889e9-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="889e9-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="889e9-158">JSON Representation</span></span>
<span data-ttu-id="889e9-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="889e9-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```




