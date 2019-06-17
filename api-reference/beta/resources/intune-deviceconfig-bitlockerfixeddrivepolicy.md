---
title: Bitlockerfixeddrive Policy リソースの種類
description: BitLocker 固定ドライブポリシー。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5729952f2700c42eaf28a292ef0f520dfbe89da
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983590"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="b3a9c-103">Bitlockerfixeddrive Policy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3a9c-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="b3a9c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3a9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3a9c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3a9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3a9c-106">BitLocker 固定ドライブポリシー。</span><span class="sxs-lookup"><span data-stu-id="b3a9c-106">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="b3a9c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3a9c-107">Properties</span></span>
|<span data-ttu-id="b3a9c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3a9c-108">Property</span></span>|<span data-ttu-id="b3a9c-109">型</span><span class="sxs-lookup"><span data-stu-id="b3a9c-109">Type</span></span>|<span data-ttu-id="b3a9c-110">説明</span><span class="sxs-lookup"><span data-stu-id="b3a9c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3a9c-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b3a9c-111">encryptionMethod</span></span>|[<span data-ttu-id="b3a9c-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b3a9c-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="b3a9c-113">固定ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="b3a9c-113">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="b3a9c-114">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="b3a9c-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="b3a9c-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="b3a9c-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="b3a9c-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3a9c-116">Boolean</span></span>|<span data-ttu-id="b3a9c-117">このポリシー設定は、固定データドライブをコンピューター上で書き込み可能にするために BitLocker 保護が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b3a9c-117">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="b3a9c-118">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="b3a9c-118">recoveryOptions</span></span>|[<span data-ttu-id="b3a9c-119">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="b3a9c-119">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="b3a9c-120">このポリシー設定を使用すると、必要な資格情報が存在しない場合に BitLocker で保護された固定データドライブを回復する方法を制御できます。</span><span class="sxs-lookup"><span data-stu-id="b3a9c-120">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="b3a9c-121">このポリシー設定は、BitLocker を有効にしたときに適用されます。</span><span class="sxs-lookup"><span data-stu-id="b3a9c-121">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3a9c-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3a9c-122">Relationships</span></span>
<span data-ttu-id="b3a9c-123">なし</span><span class="sxs-lookup"><span data-stu-id="b3a9c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3a9c-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3a9c-124">JSON Representation</span></span>
<span data-ttu-id="b3a9c-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3a9c-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerFixedDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  }
}
```





