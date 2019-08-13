---
title: EmbeddedSIMActivationCodePool の更新
description: EmbeddedSIMActivationCodePool オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f79efea881a4176640be8ebdd87b6a51cd827c9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355823"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="c90d1-103">EmbeddedSIMActivationCodePool の更新</span><span class="sxs-lookup"><span data-stu-id="c90d1-103">Update embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="c90d1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c90d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c90d1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c90d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c90d1-106">[EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c90d1-106">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c90d1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c90d1-107">Prerequisites</span></span>
<span data-ttu-id="c90d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c90d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c90d1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c90d1-110">Permission type</span></span>|<span data-ttu-id="c90d1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c90d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c90d1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c90d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c90d1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c90d1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c90d1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c90d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c90d1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c90d1-115">Not supported.</span></span>|
|<span data-ttu-id="c90d1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c90d1-116">Application</span></span>|<span data-ttu-id="c90d1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c90d1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c90d1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c90d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="c90d1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c90d1-119">Request headers</span></span>
|<span data-ttu-id="c90d1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c90d1-120">Header</span></span>|<span data-ttu-id="c90d1-121">値</span><span class="sxs-lookup"><span data-stu-id="c90d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c90d1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c90d1-122">Authorization</span></span>|<span data-ttu-id="c90d1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c90d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c90d1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c90d1-124">Accept</span></span>|<span data-ttu-id="c90d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c90d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c90d1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c90d1-126">Request body</span></span>
<span data-ttu-id="c90d1-127">要求本文で、 [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c90d1-127">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="c90d1-128">次の表に、 [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c90d1-128">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="c90d1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c90d1-129">Property</span></span>|<span data-ttu-id="c90d1-130">型</span><span class="sxs-lookup"><span data-stu-id="c90d1-130">Type</span></span>|<span data-ttu-id="c90d1-131">説明</span><span class="sxs-lookup"><span data-stu-id="c90d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c90d1-132">id</span><span class="sxs-lookup"><span data-stu-id="c90d1-132">id</span></span>|<span data-ttu-id="c90d1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c90d1-133">String</span></span>|<span data-ttu-id="c90d1-134">埋め込まれた SIM アクティブ化コードプールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c90d1-134">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="c90d1-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="c90d1-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="c90d1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c90d1-136">displayName</span></span>|<span data-ttu-id="c90d1-137">String</span><span class="sxs-lookup"><span data-stu-id="c90d1-137">String</span></span>|<span data-ttu-id="c90d1-138">埋め込まれた SIM アクティブ化コードプールの管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="c90d1-138">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="c90d1-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c90d1-139">createdDateTime</span></span>|<span data-ttu-id="c90d1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c90d1-140">DateTimeOffset</span></span>|<span data-ttu-id="c90d1-141">埋め込まれた SIM ライセンス認証コードプールが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="c90d1-141">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="c90d1-142">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="c90d1-142">Generated service side.</span></span>|
|<span data-ttu-id="c90d1-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c90d1-143">modifiedDateTime</span></span>|<span data-ttu-id="c90d1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c90d1-144">DateTimeOffset</span></span>|<span data-ttu-id="c90d1-145">埋め込まれた SIM ライセンス認証コードプールが最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="c90d1-145">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="c90d1-146">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c90d1-146">Updated service side.</span></span>|
|<span data-ttu-id="c90d1-147">activationCodes</span><span class="sxs-lookup"><span data-stu-id="c90d1-147">activationCodes</span></span>|<span data-ttu-id="c90d1-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c90d1-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="c90d1-149">このプールに属するアクティブ化コード。</span><span class="sxs-lookup"><span data-stu-id="c90d1-149">The activation codes which belong to this pool.</span></span> <span data-ttu-id="c90d1-150">このナビゲーションプロパティは、アクティブ化コードを Intune に送信するために使用されますが、Intune からのアクティブ化コードの読み取りには使用できません。</span><span class="sxs-lookup"><span data-stu-id="c90d1-150">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="c90d1-151">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="c90d1-151">activationCodeCount</span></span>|<span data-ttu-id="c90d1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c90d1-152">Int32</span></span>|<span data-ttu-id="c90d1-153">このプールに属するアクティブ化コードの合計数。</span><span class="sxs-lookup"><span data-stu-id="c90d1-153">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="c90d1-154">応答</span><span class="sxs-lookup"><span data-stu-id="c90d1-154">Response</span></span>
<span data-ttu-id="c90d1-155">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c90d1-155">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c90d1-156">例</span><span class="sxs-lookup"><span data-stu-id="c90d1-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="c90d1-157">要求</span><span class="sxs-lookup"><span data-stu-id="c90d1-157">Request</span></span>
<span data-ttu-id="c90d1-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c90d1-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
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

### <a name="response"></a><span data-ttu-id="c90d1-159">応答</span><span class="sxs-lookup"><span data-stu-id="c90d1-159">Response</span></span>
<span data-ttu-id="c90d1-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c90d1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






