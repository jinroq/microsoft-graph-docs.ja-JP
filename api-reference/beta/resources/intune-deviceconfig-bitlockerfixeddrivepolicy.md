---
title: bitLockerFixedDrivePolicy リソースの種類
description: BitLocker は、ドライブのポリシーを修正します。
ms.openlocfilehash: c29f736515333fcdbeca8c18017b9403f845de9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070310"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="c4d6e-103">bitLockerFixedDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4d6e-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="c4d6e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4d6e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4d6e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4d6e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4d6e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c4d6e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4d6e-107">BitLocker は、ドライブのポリシーを修正します。</span><span class="sxs-lookup"><span data-stu-id="c4d6e-107">BitLocker Fixed Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="c4d6e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4d6e-108">Properties</span></span>
|<span data-ttu-id="c4d6e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4d6e-109">Property</span></span>|<span data-ttu-id="c4d6e-110">型</span><span class="sxs-lookup"><span data-stu-id="c4d6e-110">Type</span></span>|<span data-ttu-id="c4d6e-111">説明</span><span class="sxs-lookup"><span data-stu-id="c4d6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4d6e-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="c4d6e-112">encryptionMethod</span></span>|[<span data-ttu-id="c4d6e-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="c4d6e-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="c4d6e-114">固定のドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="c4d6e-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="c4d6e-115">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="c4d6e-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="c4d6e-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="c4d6e-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="c4d6e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4d6e-117">Boolean</span></span>|<span data-ttu-id="c4d6e-118">このポリシー設定は、BitLocker の保護が固定データ ドライブをコンピューターに書き込み可能にするために必要かどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="c4d6e-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="c4d6e-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="c4d6e-119">recoveryOptions</span></span>|[<span data-ttu-id="c4d6e-120">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="c4d6e-120">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="c4d6e-121">このポリシー設定では、BitLocker で保護された方法固定データ ドライブは、必要な資格情報がない場合にリカバリを制御できます。</span><span class="sxs-lookup"><span data-stu-id="c4d6e-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="c4d6e-122">BitLocker を有効にするときは、このポリシー設定が適用されます。</span><span class="sxs-lookup"><span data-stu-id="c4d6e-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4d6e-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c4d6e-123">Relationships</span></span>
<span data-ttu-id="c4d6e-124">なし</span><span class="sxs-lookup"><span data-stu-id="c4d6e-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4d6e-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4d6e-125">JSON Representation</span></span>
<span data-ttu-id="c4d6e-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c4d6e-126">Here is a JSON representation of the resource.</span></span>
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





