---
title: userPFXCertificate リソースの種類
description: PFX 証明書のユーザーのために必要なすべての情報をカプセル化するエンティティです。
localization_priority: Normal
ms.openlocfilehash: 87516c48e53c8117c9efa119fb6cab62844e6b68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809997"
---
# <a name="userpfxcertificate-resource-type"></a><span data-ttu-id="27596-103">userPFXCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27596-103">userPFXCertificate resource type</span></span>

> <span data-ttu-id="27596-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="27596-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27596-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27596-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27596-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="27596-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27596-107">PFX 証明書のユーザーのために必要なすべての情報をカプセル化するエンティティです。</span><span class="sxs-lookup"><span data-stu-id="27596-107">Entity that encapsulates all information required for a user's PFX certificates.</span></span>
## <a name="methods"></a><span data-ttu-id="27596-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="27596-108">Methods</span></span>
|<span data-ttu-id="27596-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="27596-109">Method</span></span>|<span data-ttu-id="27596-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="27596-110">Return Type</span></span>|<span data-ttu-id="27596-111">説明</span><span class="sxs-lookup"><span data-stu-id="27596-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27596-112">リスト userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="27596-112">List userPFXCertificates</span></span>](../api/intune-raimportcerts-userpfxcertificate-list.md)|<span data-ttu-id="27596-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="27596-113">[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) collection</span></span>|<span data-ttu-id="27596-114">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="27596-114">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>|
|[<span data-ttu-id="27596-115">UserPFXCertificate を取得します。</span><span class="sxs-lookup"><span data-stu-id="27596-115">Get userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-get.md)|[<span data-ttu-id="27596-116">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="27596-116">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="27596-117">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27596-117">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="27596-118">UserPFXCertificate を作成します。</span><span class="sxs-lookup"><span data-stu-id="27596-118">Create userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-create.md)|[<span data-ttu-id="27596-119">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="27596-119">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="27596-120">新しい[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="27596-120">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|
|[<span data-ttu-id="27596-121">UserPFXCertificate を削除します。</span><span class="sxs-lookup"><span data-stu-id="27596-121">Delete userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-delete.md)|<span data-ttu-id="27596-122">なし</span><span class="sxs-lookup"><span data-stu-id="27596-122">None</span></span>|<span data-ttu-id="27596-123">の[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="27596-123">Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>|
|[<span data-ttu-id="27596-124">UserPFXCertificate を更新します。</span><span class="sxs-lookup"><span data-stu-id="27596-124">Update userPFXCertificate</span></span>](../api/intune-raimportcerts-userpfxcertificate-update.md)|[<span data-ttu-id="27596-125">userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="27596-125">userPFXCertificate</span></span>](../resources/intune-raimportcerts-userpfxcertificate.md)|<span data-ttu-id="27596-126">[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="27596-126">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27596-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27596-127">Properties</span></span>
|<span data-ttu-id="27596-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27596-128">Property</span></span>|<span data-ttu-id="27596-129">種類</span><span class="sxs-lookup"><span data-stu-id="27596-129">Type</span></span>|<span data-ttu-id="27596-130">説明</span><span class="sxs-lookup"><span data-stu-id="27596-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27596-131">ID</span><span class="sxs-lookup"><span data-stu-id="27596-131">id</span></span>|<span data-ttu-id="27596-132">String</span><span class="sxs-lookup"><span data-stu-id="27596-132">String</span></span>|<span data-ttu-id="27596-133">PFX 証明書の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="27596-133">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="27596-134">拇印</span><span class="sxs-lookup"><span data-stu-id="27596-134">thumbprint</span></span>|<span data-ttu-id="27596-135">String</span><span class="sxs-lookup"><span data-stu-id="27596-135">String</span></span>|<span data-ttu-id="27596-136">PFX 証明書の拇印を sha-1 です。</span><span class="sxs-lookup"><span data-stu-id="27596-136">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="27596-137">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="27596-137">intendedPurpose</span></span>|[<span data-ttu-id="27596-138">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="27596-138">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="27596-139">証明書からのポイントからのビューの展開の目的のものです。</span><span class="sxs-lookup"><span data-stu-id="27596-139">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="27596-140">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="27596-140">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="27596-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="27596-141">userPrincipalName</span></span>|<span data-ttu-id="27596-142">String</span><span class="sxs-lookup"><span data-stu-id="27596-142">String</span></span>|<span data-ttu-id="27596-143">PFX 証明書のユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="27596-143">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="27596-144">startDateTime</span><span class="sxs-lookup"><span data-stu-id="27596-144">startDateTime</span></span>|<span data-ttu-id="27596-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27596-145">DateTimeOffset</span></span>|<span data-ttu-id="27596-146">証明書の有効性は、日付と時刻を開始します。</span><span class="sxs-lookup"><span data-stu-id="27596-146">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="27596-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="27596-147">expirationDateTime</span></span>|<span data-ttu-id="27596-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27596-148">DateTimeOffset</span></span>|<span data-ttu-id="27596-149">証明書の有効期限切れ日時です。</span><span class="sxs-lookup"><span data-stu-id="27596-149">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="27596-150">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="27596-150">providerName</span></span>|<span data-ttu-id="27596-151">String</span><span class="sxs-lookup"><span data-stu-id="27596-151">String</span></span>|<span data-ttu-id="27596-152">暗号サービス プロバイダーがこの blob の暗号化に使用します。</span><span class="sxs-lookup"><span data-stu-id="27596-152">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="27596-153">キー名</span><span class="sxs-lookup"><span data-stu-id="27596-153">keyName</span></span>|<span data-ttu-id="27596-154">String</span><span class="sxs-lookup"><span data-stu-id="27596-154">String</span></span>|<span data-ttu-id="27596-155">(プロバイダー) 内のキーの名前が blob の暗号化に使用します。</span><span class="sxs-lookup"><span data-stu-id="27596-155">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="27596-156">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="27596-156">paddingScheme</span></span>|[<span data-ttu-id="27596-157">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="27596-157">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="27596-158">暗号化/復号化中に、プロバイダーによって使用されるスキームをパディングします。</span><span class="sxs-lookup"><span data-stu-id="27596-158">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="27596-159">使用可能な値: `none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="27596-159">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="27596-160">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="27596-160">encryptedPfxBlob</span></span>|<span data-ttu-id="27596-161">Binary</span><span class="sxs-lookup"><span data-stu-id="27596-161">Binary</span></span>|<span data-ttu-id="27596-162">PFX の暗号化された blob です。</span><span class="sxs-lookup"><span data-stu-id="27596-162">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="27596-163">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="27596-163">encryptedPfxPassword</span></span>|<span data-ttu-id="27596-164">String</span><span class="sxs-lookup"><span data-stu-id="27596-164">String</span></span>|<span data-ttu-id="27596-165">PFX パスワードを暗号化します。</span><span class="sxs-lookup"><span data-stu-id="27596-165">Encrypted PFX password.</span></span>|
|<span data-ttu-id="27596-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27596-166">createdDateTime</span></span>|<span data-ttu-id="27596-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27596-167">DateTimeOffset</span></span>|<span data-ttu-id="27596-168">PFX 証明書がインポートされたときに、日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="27596-168">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="27596-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27596-169">lastModifiedDateTime</span></span>|<span data-ttu-id="27596-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27596-170">DateTimeOffset</span></span>|<span data-ttu-id="27596-171">PFX 証明書が最後に修正された日時です。</span><span class="sxs-lookup"><span data-stu-id="27596-171">Date/time when this PFX certificate was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27596-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="27596-172">Relationships</span></span>
<span data-ttu-id="27596-173">なし</span><span class="sxs-lookup"><span data-stu-id="27596-173">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27596-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27596-174">JSON Representation</span></span>
<span data-ttu-id="27596-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="27596-175">Here is a JSON representation of the resource.</span></span>
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





