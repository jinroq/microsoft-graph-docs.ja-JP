---
title: userPFXCertificate リソースの種類
description: PFX 証明書のユーザーのために必要なすべての情報をカプセル化するエンティティです。
ms.openlocfilehash: 89040cafa976c88ce84cb8f73bc8a68e2cdfbdf2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070921"
---
# <a name="userpfxcertificate-resource-type"></a><span data-ttu-id="c0b04-103">userPFXCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0b04-103">userPFXCertificate resource type</span></span>

> <span data-ttu-id="c0b04-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0b04-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0b04-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0b04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0b04-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0b04-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0b04-107">PFX 証明書のユーザーのために必要なすべての情報をカプセル化するエンティティです。</span><span class="sxs-lookup"><span data-stu-id="c0b04-107">Entity that encapsulates all information required for a user's PFX certificates.</span></span>
## <a name="methods"></a><span data-ttu-id="c0b04-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c0b04-108">Methods</span></span>
|<span data-ttu-id="c0b04-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c0b04-109">Method</span></span>|<span data-ttu-id="c0b04-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c0b04-110">Return Type</span></span>|<span data-ttu-id="c0b04-111">説明</span><span class="sxs-lookup"><span data-stu-id="c0b04-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0b04-112">リスト userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="c0b04-112">List userPFXCertificates</span></span>](../api/intune-raimportcerts-userpfxcertificate-list.md)|<span data-ttu-id="c0b04-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c0b04-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) collection</span></span>|<span data-ttu-id="c0b04-114">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-114">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>|
|[<span data-ttu-id="c0b04-115">UserPFXCertificate を取得します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-115">Get userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-get.md)|[<span data-ttu-id="c0b04-116">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="c0b04-116">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="c0b04-117">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0b04-117">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="c0b04-118">UserPFXCertificate を作成します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-118">Create userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-create.md)|[<span data-ttu-id="c0b04-119">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="c0b04-119">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="c0b04-120">新しい[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-120">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="c0b04-121">UserPFXCertificate を削除します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-121">Delete userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-delete.md)|<span data-ttu-id="c0b04-122">なし</span><span class="sxs-lookup"><span data-stu-id="c0b04-122">None</span></span>|<span data-ttu-id="c0b04-123">の[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-123">Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>|
|[<span data-ttu-id="c0b04-124">UserPFXCertificate を更新します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-124">Update userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-update.md)|[<span data-ttu-id="c0b04-125">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="c0b04-125">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="c0b04-126">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-126">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0b04-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0b04-127">Properties</span></span>
|<span data-ttu-id="c0b04-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0b04-128">Property</span></span>|<span data-ttu-id="c0b04-129">型</span><span class="sxs-lookup"><span data-stu-id="c0b04-129">Type</span></span>|<span data-ttu-id="c0b04-130">説明</span><span class="sxs-lookup"><span data-stu-id="c0b04-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0b04-131">id</span><span class="sxs-lookup"><span data-stu-id="c0b04-131">id</span></span>|<span data-ttu-id="c0b04-132">String</span><span class="sxs-lookup"><span data-stu-id="c0b04-132">String</span></span>|<span data-ttu-id="c0b04-133">PFX 証明書の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c0b04-133">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="c0b04-134">拇印</span><span class="sxs-lookup"><span data-stu-id="c0b04-134">thumbprint</span></span>|<span data-ttu-id="c0b04-135">String</span><span class="sxs-lookup"><span data-stu-id="c0b04-135">String</span></span>|<span data-ttu-id="c0b04-136">PFX 証明書の拇印を sha-1 です。</span><span class="sxs-lookup"><span data-stu-id="c0b04-136">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="c0b04-137">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="c0b04-137">intendedPurpose</span></span>|[<span data-ttu-id="c0b04-138">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="c0b04-138">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="c0b04-139">証明書からのポイントからのビューの展開の目的のものです。</span><span class="sxs-lookup"><span data-stu-id="c0b04-139">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="c0b04-140">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="c0b04-140">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="c0b04-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c0b04-141">userPrincipalName</span></span>|<span data-ttu-id="c0b04-142">String</span><span class="sxs-lookup"><span data-stu-id="c0b04-142">String</span></span>|<span data-ttu-id="c0b04-143">PFX 証明書のユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="c0b04-143">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="c0b04-144">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b04-144">startDateTime</span></span>|<span data-ttu-id="c0b04-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b04-145">DateTimeOffset</span></span>|<span data-ttu-id="c0b04-146">証明書の有効性は、日付と時刻を開始します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-146">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="c0b04-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b04-147">expirationDateTime</span></span>|<span data-ttu-id="c0b04-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b04-148">DateTimeOffset</span></span>|<span data-ttu-id="c0b04-149">証明書の有効期限切れ日時です。</span><span class="sxs-lookup"><span data-stu-id="c0b04-149">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="c0b04-150">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="c0b04-150">providerName</span></span>|<span data-ttu-id="c0b04-151">String</span><span class="sxs-lookup"><span data-stu-id="c0b04-151">String</span></span>|<span data-ttu-id="c0b04-152">暗号サービス プロバイダーがこの blob の暗号化に使用します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-152">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="c0b04-153">キー名</span><span class="sxs-lookup"><span data-stu-id="c0b04-153">keyName</span></span>|<span data-ttu-id="c0b04-154">String</span><span class="sxs-lookup"><span data-stu-id="c0b04-154">String</span></span>|<span data-ttu-id="c0b04-155">(プロバイダー) 内のキーの名前が blob の暗号化に使用します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-155">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="c0b04-156">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="c0b04-156">paddingScheme</span></span>|[<span data-ttu-id="c0b04-157">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="c0b04-157">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="c0b04-158">暗号化/復号化中に、プロバイダーによって使用されるスキームをパディングします。</span><span class="sxs-lookup"><span data-stu-id="c0b04-158">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="c0b04-159">使用可能な値: `none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="c0b04-159">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="c0b04-160">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="c0b04-160">encryptedPfxBlob</span></span>|<span data-ttu-id="c0b04-161">バイナリ</span><span class="sxs-lookup"><span data-stu-id="c0b04-161">Binary</span></span>|<span data-ttu-id="c0b04-162">PFX の暗号化された blob です。</span><span class="sxs-lookup"><span data-stu-id="c0b04-162">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="c0b04-163">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="c0b04-163">encryptedPfxPassword</span></span>|<span data-ttu-id="c0b04-164">String</span><span class="sxs-lookup"><span data-stu-id="c0b04-164">String</span></span>|<span data-ttu-id="c0b04-165">PFX パスワードを暗号化します。</span><span class="sxs-lookup"><span data-stu-id="c0b04-165">Encrypted PFX password.</span></span>|
|<span data-ttu-id="c0b04-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b04-166">createdDateTime</span></span>|<span data-ttu-id="c0b04-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b04-167">DateTimeOffset</span></span>|<span data-ttu-id="c0b04-168">PFX 証明書がインポートされたときに、日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c0b04-168">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="c0b04-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b04-169">lastModifiedDateTime</span></span>|<span data-ttu-id="c0b04-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b04-170">DateTimeOffset</span></span>|<span data-ttu-id="c0b04-171">PFX 証明書が最後に修正された日時です。</span><span class="sxs-lookup"><span data-stu-id="c0b04-171">Date/time when this PFX certificate was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0b04-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c0b04-172">Relationships</span></span>
<span data-ttu-id="c0b04-173">なし</span><span class="sxs-lookup"><span data-stu-id="c0b04-173">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c0b04-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0b04-174">JSON Representation</span></span>
<span data-ttu-id="c0b04-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0b04-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userPFXCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "String (identifier)",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





