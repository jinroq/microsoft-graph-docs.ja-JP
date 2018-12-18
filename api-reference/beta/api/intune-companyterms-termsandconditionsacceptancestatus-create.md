---
title: termsAndConditionsAcceptanceStatus の作成
description: 新しい termsAndConditionsAcceptanceStatus オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 857e927d970f91070032dae95e699247aa7b11b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340594"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="81b5a-103">termsAndConditionsAcceptanceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="81b5a-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="81b5a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81b5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81b5a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81b5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81b5a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81b5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81b5a-107">新しい [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="81b5a-107">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81b5a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="81b5a-108">Prerequisites</span></span>
<span data-ttu-id="81b5a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81b5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81b5a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81b5a-111">Permission type</span></span>|<span data-ttu-id="81b5a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="81b5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81b5a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81b5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81b5a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81b5a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="81b5a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81b5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81b5a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81b5a-116">Not supported.</span></span>|
|<span data-ttu-id="81b5a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81b5a-117">Application</span></span>|<span data-ttu-id="81b5a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81b5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81b5a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81b5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="81b5a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81b5a-120">Request headers</span></span>
|<span data-ttu-id="81b5a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81b5a-121">Header</span></span>|<span data-ttu-id="81b5a-122">値</span><span class="sxs-lookup"><span data-stu-id="81b5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81b5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="81b5a-123">Authorization</span></span>|<span data-ttu-id="81b5a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="81b5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81b5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="81b5a-125">Accept</span></span>|<span data-ttu-id="81b5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81b5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81b5a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="81b5a-127">Request body</span></span>
<span data-ttu-id="81b5a-128">要求本文で、termsAndConditionsAcceptanceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="81b5a-128">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="81b5a-129">次の表に、termsAndConditionsAcceptanceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="81b5a-129">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="81b5a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81b5a-130">Property</span></span>|<span data-ttu-id="81b5a-131">種類</span><span class="sxs-lookup"><span data-stu-id="81b5a-131">Type</span></span>|<span data-ttu-id="81b5a-132">説明</span><span class="sxs-lookup"><span data-stu-id="81b5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81b5a-133">ID</span><span class="sxs-lookup"><span data-stu-id="81b5a-133">id</span></span>|<span data-ttu-id="81b5a-134">String</span><span class="sxs-lookup"><span data-stu-id="81b5a-134">String</span></span>|<span data-ttu-id="81b5a-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="81b5a-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="81b5a-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="81b5a-136">userDisplayName</span></span>|<span data-ttu-id="81b5a-137">String</span><span class="sxs-lookup"><span data-stu-id="81b5a-137">String</span></span>|<span data-ttu-id="81b5a-138">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="81b5a-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="81b5a-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="81b5a-139">acceptedVersion</span></span>|<span data-ttu-id="81b5a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="81b5a-140">Int32</span></span>|<span data-ttu-id="81b5a-141">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="81b5a-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="81b5a-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="81b5a-142">acceptedDateTime</span></span>|<span data-ttu-id="81b5a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81b5a-143">DateTimeOffset</span></span>|<span data-ttu-id="81b5a-144">最後にユーザーによって使用条件が承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="81b5a-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="81b5a-145">応答</span><span class="sxs-lookup"><span data-stu-id="81b5a-145">Response</span></span>
<span data-ttu-id="81b5a-146">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="81b5a-146">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81b5a-147">例</span><span class="sxs-lookup"><span data-stu-id="81b5a-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="81b5a-148">要求</span><span class="sxs-lookup"><span data-stu-id="81b5a-148">Request</span></span>
<span data-ttu-id="81b5a-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81b5a-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="81b5a-150">応答</span><span class="sxs-lookup"><span data-stu-id="81b5a-150">Response</span></span>
<span data-ttu-id="81b5a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81b5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```





