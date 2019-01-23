---
title: EmbeddedSIMActivationCodePool を更新します。
description: EmbeddedSIMActivationCodePool オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1894e0702f2d49cff86e9b7510c94eac5cbd0134
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404443"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="0d842-103">EmbeddedSIMActivationCodePool を更新します。</span><span class="sxs-lookup"><span data-stu-id="0d842-103">Update embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="0d842-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0d842-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0d842-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d842-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d842-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d842-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d842-107">[EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0d842-107">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d842-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0d842-108">Prerequisites</span></span>
<span data-ttu-id="0d842-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d842-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0d842-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d842-111">Permission type</span></span>|<span data-ttu-id="0d842-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d842-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d842-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d842-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d842-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d842-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d842-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d842-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d842-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d842-116">Not supported.</span></span>|
|<span data-ttu-id="0d842-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d842-117">Application</span></span>|<span data-ttu-id="0d842-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d842-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d842-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d842-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="0d842-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d842-120">Request headers</span></span>
|<span data-ttu-id="0d842-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d842-121">Header</span></span>|<span data-ttu-id="0d842-122">値</span><span class="sxs-lookup"><span data-stu-id="0d842-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d842-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d842-123">Authorization</span></span>|<span data-ttu-id="0d842-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0d842-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d842-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0d842-125">Accept</span></span>|<span data-ttu-id="0d842-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d842-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d842-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d842-127">Request body</span></span>
<span data-ttu-id="0d842-128">要求の本文に[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0d842-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="0d842-129">[EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="0d842-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="0d842-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d842-130">Property</span></span>|<span data-ttu-id="0d842-131">型</span><span class="sxs-lookup"><span data-stu-id="0d842-131">Type</span></span>|<span data-ttu-id="0d842-132">説明</span><span class="sxs-lookup"><span data-stu-id="0d842-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d842-133">id</span><span class="sxs-lookup"><span data-stu-id="0d842-133">id</span></span>|<span data-ttu-id="0d842-134">String</span><span class="sxs-lookup"><span data-stu-id="0d842-134">String</span></span>|<span data-ttu-id="0d842-135">SIM のアクティブ化コードの埋め込み、プールの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="0d842-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="0d842-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="0d842-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0d842-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0d842-137">displayName</span></span>|<span data-ttu-id="0d842-138">String</span><span class="sxs-lookup"><span data-stu-id="0d842-138">String</span></span>|<span data-ttu-id="0d842-139">管理者には、埋め込み SIM アクティベーション コードのプールの名前が定義されています。</span><span class="sxs-lookup"><span data-stu-id="0d842-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="0d842-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d842-140">createdDateTime</span></span>|<span data-ttu-id="0d842-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d842-141">DateTimeOffset</span></span>|<span data-ttu-id="0d842-142">埋め込み SIM アクティベーション コードのプールが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="0d842-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="0d842-143">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="0d842-143">Generated service side.</span></span>|
|<span data-ttu-id="0d842-144">変更された日時</span><span class="sxs-lookup"><span data-stu-id="0d842-144">modifiedDateTime</span></span>|<span data-ttu-id="0d842-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d842-145">DateTimeOffset</span></span>|<span data-ttu-id="0d842-146">埋め込み SIM アクティベーション コードのプールが最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="0d842-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="0d842-147">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="0d842-147">Updated service side.</span></span>|
|<span data-ttu-id="0d842-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="0d842-148">activationCodes</span></span>|<span data-ttu-id="0d842-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0d842-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="0d842-150">このプールに属しているアクティブ化コードです。</span><span class="sxs-lookup"><span data-stu-id="0d842-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="0d842-151">このナビゲーション プロパティは Intune にライセンス認証コードを投稿するために使用しますが、Intune からアクティブ化コードを読み取るには使用できません。</span><span class="sxs-lookup"><span data-stu-id="0d842-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="0d842-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="0d842-152">activationCodeCount</span></span>|<span data-ttu-id="0d842-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0d842-153">Int32</span></span>|<span data-ttu-id="0d842-154">このプールに属しているアクティブ化コードの合計数。</span><span class="sxs-lookup"><span data-stu-id="0d842-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="0d842-155">応答</span><span class="sxs-lookup"><span data-stu-id="0d842-155">Response</span></span>
<span data-ttu-id="0d842-156">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0d842-156">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d842-157">例</span><span class="sxs-lookup"><span data-stu-id="0d842-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d842-158">要求</span><span class="sxs-lookup"><span data-stu-id="0d842-158">Request</span></span>
<span data-ttu-id="0d842-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0d842-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d842-160">応答</span><span class="sxs-lookup"><span data-stu-id="0d842-160">Response</span></span>
<span data-ttu-id="0d842-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d842-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




