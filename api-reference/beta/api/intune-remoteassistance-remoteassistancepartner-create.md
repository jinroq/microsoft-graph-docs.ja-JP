---
title: remoteAssistancePartner の作成
description: 新しい remoteAssistancePartner オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b1f8306c3ece3b5153a9352c38e41eb89e71d6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410428"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="5f25c-103">remoteAssistancePartner の作成</span><span class="sxs-lookup"><span data-stu-id="5f25c-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="5f25c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5f25c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5f25c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f25c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f25c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5f25c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f25c-107">新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5f25c-107">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f25c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5f25c-108">Prerequisites</span></span>
<span data-ttu-id="5f25c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f25c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5f25c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f25c-111">Permission type</span></span>|<span data-ttu-id="5f25c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f25c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f25c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f25c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f25c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f25c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5f25c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f25c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f25c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f25c-116">Not supported.</span></span>|
|<span data-ttu-id="5f25c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f25c-117">Application</span></span>|<span data-ttu-id="5f25c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f25c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f25c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f25c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="5f25c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f25c-120">Request headers</span></span>
|<span data-ttu-id="5f25c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f25c-121">Header</span></span>|<span data-ttu-id="5f25c-122">値</span><span class="sxs-lookup"><span data-stu-id="5f25c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f25c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f25c-123">Authorization</span></span>|<span data-ttu-id="5f25c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5f25c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f25c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5f25c-125">Accept</span></span>|<span data-ttu-id="5f25c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f25c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f25c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f25c-127">Request body</span></span>
<span data-ttu-id="5f25c-128">要求本文で、remoteAssistancePartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5f25c-128">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="5f25c-129">次の表に、remoteAssistancePartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5f25c-129">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="5f25c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f25c-130">Property</span></span>|<span data-ttu-id="5f25c-131">型</span><span class="sxs-lookup"><span data-stu-id="5f25c-131">Type</span></span>|<span data-ttu-id="5f25c-132">説明</span><span class="sxs-lookup"><span data-stu-id="5f25c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f25c-133">id</span><span class="sxs-lookup"><span data-stu-id="5f25c-133">id</span></span>|<span data-ttu-id="5f25c-134">String</span><span class="sxs-lookup"><span data-stu-id="5f25c-134">String</span></span>|<span data-ttu-id="5f25c-135">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5f25c-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="5f25c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5f25c-136">displayName</span></span>|<span data-ttu-id="5f25c-137">String</span><span class="sxs-lookup"><span data-stu-id="5f25c-137">String</span></span>|<span data-ttu-id="5f25c-138">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="5f25c-138">Display name of the partner.</span></span>|
|<span data-ttu-id="5f25c-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="5f25c-139">onboardingUrl</span></span>|<span data-ttu-id="5f25c-140">String</span><span class="sxs-lookup"><span data-stu-id="5f25c-140">String</span></span>|<span data-ttu-id="5f25c-141">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="5f25c-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="5f25c-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="5f25c-142">onboardingStatus</span></span>|[<span data-ttu-id="5f25c-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="5f25c-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="5f25c-144">未定です。</span><span class="sxs-lookup"><span data-stu-id="5f25c-144">TBD.</span></span> <span data-ttu-id="5f25c-145">可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="5f25c-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="5f25c-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="5f25c-146">lastConnectionDateTime</span></span>|<span data-ttu-id="5f25c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f25c-147">DateTimeOffset</span></span>|<span data-ttu-id="5f25c-148">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="5f25c-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="5f25c-149">応答</span><span class="sxs-lookup"><span data-stu-id="5f25c-149">Response</span></span>
<span data-ttu-id="5f25c-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5f25c-150">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f25c-151">例</span><span class="sxs-lookup"><span data-stu-id="5f25c-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f25c-152">要求</span><span class="sxs-lookup"><span data-stu-id="5f25c-152">Request</span></span>
<span data-ttu-id="5f25c-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f25c-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="5f25c-154">応答</span><span class="sxs-lookup"><span data-stu-id="5f25c-154">Response</span></span>
<span data-ttu-id="5f25c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5f25c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```




