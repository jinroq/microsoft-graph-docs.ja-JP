---
title: embeddedSIMActivationCodePool を作成する
description: 新しい embeddedSIMActivationCodePool オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1fc25e95f961630b19b022c4156ef0b6ec2059b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532437"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="9ccf9-103">embeddedSIMActivationCodePool を作成する</span><span class="sxs-lookup"><span data-stu-id="9ccf9-103">Create embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="9ccf9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ccf9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ccf9-106">新しい[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-106">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ccf9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9ccf9-107">Prerequisites</span></span>
<span data-ttu-id="9ccf9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ccf9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ccf9-110">Permission type</span></span>|<span data-ttu-id="9ccf9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ccf9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ccf9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ccf9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ccf9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ccf9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ccf9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ccf9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ccf9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-115">Not supported.</span></span>|
|<span data-ttu-id="9ccf9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ccf9-116">Application</span></span>|<span data-ttu-id="9ccf9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ccf9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ccf9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="9ccf9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ccf9-119">Request headers</span></span>
|<span data-ttu-id="9ccf9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ccf9-120">Header</span></span>|<span data-ttu-id="9ccf9-121">値</span><span class="sxs-lookup"><span data-stu-id="9ccf9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ccf9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ccf9-122">Authorization</span></span>|<span data-ttu-id="9ccf9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ccf9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9ccf9-124">Accept</span></span>|<span data-ttu-id="9ccf9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ccf9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ccf9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ccf9-126">Request body</span></span>
<span data-ttu-id="9ccf9-127">要求本文で、embeddedSIMActivationCodePool オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-127">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="9ccf9-128">次の表に、embeddedSIMActivationCodePool の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-128">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="9ccf9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ccf9-129">Property</span></span>|<span data-ttu-id="9ccf9-130">型</span><span class="sxs-lookup"><span data-stu-id="9ccf9-130">Type</span></span>|<span data-ttu-id="9ccf9-131">説明</span><span class="sxs-lookup"><span data-stu-id="9ccf9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ccf9-132">id</span><span class="sxs-lookup"><span data-stu-id="9ccf9-132">id</span></span>|<span data-ttu-id="9ccf9-133">String</span><span class="sxs-lookup"><span data-stu-id="9ccf9-133">String</span></span>|<span data-ttu-id="9ccf9-134">埋め込まれた SIM アクティブ化コードプールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-134">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="9ccf9-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="9ccf9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9ccf9-136">displayName</span></span>|<span data-ttu-id="9ccf9-137">String</span><span class="sxs-lookup"><span data-stu-id="9ccf9-137">String</span></span>|<span data-ttu-id="9ccf9-138">埋め込まれた SIM アクティブ化コードプールの管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-138">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="9ccf9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ccf9-139">createdDateTime</span></span>|<span data-ttu-id="9ccf9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ccf9-140">DateTimeOffset</span></span>|<span data-ttu-id="9ccf9-141">埋め込まれた SIM ライセンス認証コードプールが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-141">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="9ccf9-142">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-142">Generated service side.</span></span>|
|<span data-ttu-id="9ccf9-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ccf9-143">modifiedDateTime</span></span>|<span data-ttu-id="9ccf9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ccf9-144">DateTimeOffset</span></span>|<span data-ttu-id="9ccf9-145">埋め込まれた SIM ライセンス認証コードプールが最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-145">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="9ccf9-146">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-146">Updated service side.</span></span>|
|<span data-ttu-id="9ccf9-147">activationCodes</span><span class="sxs-lookup"><span data-stu-id="9ccf9-147">activationCodes</span></span>|<span data-ttu-id="9ccf9-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9ccf9-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="9ccf9-149">このプールに属するアクティブ化コード。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-149">The activation codes which belong to this pool.</span></span> <span data-ttu-id="9ccf9-150">このナビゲーションプロパティは、アクティブ化コードを intune に送信するために使用されますが、intune からのアクティブ化コードの読み取りには使用できません。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-150">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="9ccf9-151">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="9ccf9-151">activationCodeCount</span></span>|<span data-ttu-id="9ccf9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9ccf9-152">Int32</span></span>|<span data-ttu-id="9ccf9-153">このプールに属するアクティブ化コードの合計数。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-153">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="9ccf9-154">応答</span><span class="sxs-lookup"><span data-stu-id="9ccf9-154">Response</span></span>
<span data-ttu-id="9ccf9-155">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-155">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ccf9-156">例</span><span class="sxs-lookup"><span data-stu-id="9ccf9-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ccf9-157">要求</span><span class="sxs-lookup"><span data-stu-id="9ccf9-157">Request</span></span>
<span data-ttu-id="9ccf9-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a><span data-ttu-id="9ccf9-159">応答</span><span class="sxs-lookup"><span data-stu-id="9ccf9-159">Response</span></span>
<span data-ttu-id="9ccf9-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9ccf9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```





