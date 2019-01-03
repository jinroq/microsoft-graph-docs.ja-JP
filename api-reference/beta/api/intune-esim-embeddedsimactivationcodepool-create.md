---
title: EmbeddedSIMActivationCodePool を作成します。
description: 新しい embeddedSIMActivationCodePool オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 88b495437859e6e7552763581886e0bf6786374c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302598"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="9db46-103">EmbeddedSIMActivationCodePool を作成します。</span><span class="sxs-lookup"><span data-stu-id="9db46-103">Create embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="9db46-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9db46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9db46-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9db46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9db46-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9db46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9db46-107">新しい[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9db46-107">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9db46-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9db46-108">Prerequisites</span></span>
<span data-ttu-id="9db46-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9db46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9db46-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9db46-111">Permission type</span></span>|<span data-ttu-id="9db46-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9db46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9db46-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9db46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9db46-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9db46-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9db46-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9db46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9db46-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9db46-116">Not supported.</span></span>|
|<span data-ttu-id="9db46-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9db46-117">Application</span></span>|<span data-ttu-id="9db46-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9db46-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9db46-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9db46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="9db46-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9db46-120">Request headers</span></span>
|<span data-ttu-id="9db46-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9db46-121">Header</span></span>|<span data-ttu-id="9db46-122">値</span><span class="sxs-lookup"><span data-stu-id="9db46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9db46-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9db46-123">Authorization</span></span>|<span data-ttu-id="9db46-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9db46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9db46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9db46-125">Accept</span></span>|<span data-ttu-id="9db46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9db46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9db46-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9db46-127">Request body</span></span>
<span data-ttu-id="9db46-128">要求の本文に embeddedSIMActivationCodePool オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9db46-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="9db46-129">次の表は、embeddedSIMActivationCodePool を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9db46-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="9db46-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9db46-130">Property</span></span>|<span data-ttu-id="9db46-131">種類</span><span class="sxs-lookup"><span data-stu-id="9db46-131">Type</span></span>|<span data-ttu-id="9db46-132">説明</span><span class="sxs-lookup"><span data-stu-id="9db46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9db46-133">ID</span><span class="sxs-lookup"><span data-stu-id="9db46-133">id</span></span>|<span data-ttu-id="9db46-134">String</span><span class="sxs-lookup"><span data-stu-id="9db46-134">String</span></span>|<span data-ttu-id="9db46-135">SIM のアクティブ化コードの埋め込み、プールの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="9db46-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="9db46-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="9db46-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="9db46-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9db46-137">displayName</span></span>|<span data-ttu-id="9db46-138">String</span><span class="sxs-lookup"><span data-stu-id="9db46-138">String</span></span>|<span data-ttu-id="9db46-139">管理者には、埋め込み SIM アクティベーション コードのプールの名前が定義されています。</span><span class="sxs-lookup"><span data-stu-id="9db46-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="9db46-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9db46-140">createdDateTime</span></span>|<span data-ttu-id="9db46-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9db46-141">DateTimeOffset</span></span>|<span data-ttu-id="9db46-142">埋め込み SIM アクティベーション コードのプールが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="9db46-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="9db46-143">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="9db46-143">Generated service side.</span></span>|
|<span data-ttu-id="9db46-144">変更された日時</span><span class="sxs-lookup"><span data-stu-id="9db46-144">modifiedDateTime</span></span>|<span data-ttu-id="9db46-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9db46-145">DateTimeOffset</span></span>|<span data-ttu-id="9db46-146">埋め込み SIM アクティベーション コードのプールが最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="9db46-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="9db46-147">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="9db46-147">Updated service side.</span></span>|
|<span data-ttu-id="9db46-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="9db46-148">activationCodes</span></span>|<span data-ttu-id="9db46-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9db46-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="9db46-150">このプールに属しているアクティブ化コードです。</span><span class="sxs-lookup"><span data-stu-id="9db46-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="9db46-151">このナビゲーション プロパティは Intune にライセンス認証コードを投稿するために使用しますが、Intune からアクティブ化コードを読み取るには使用できません。</span><span class="sxs-lookup"><span data-stu-id="9db46-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="9db46-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="9db46-152">activationCodeCount</span></span>|<span data-ttu-id="9db46-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9db46-153">Int32</span></span>|<span data-ttu-id="9db46-154">このプールに属しているアクティブ化コードの合計数。</span><span class="sxs-lookup"><span data-stu-id="9db46-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="9db46-155">応答</span><span class="sxs-lookup"><span data-stu-id="9db46-155">Response</span></span>
<span data-ttu-id="9db46-156">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9db46-156">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9db46-157">例</span><span class="sxs-lookup"><span data-stu-id="9db46-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="9db46-158">要求</span><span class="sxs-lookup"><span data-stu-id="9db46-158">Request</span></span>
<span data-ttu-id="9db46-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9db46-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9db46-160">応答</span><span class="sxs-lookup"><span data-stu-id="9db46-160">Response</span></span>
<span data-ttu-id="9db46-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9db46-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




