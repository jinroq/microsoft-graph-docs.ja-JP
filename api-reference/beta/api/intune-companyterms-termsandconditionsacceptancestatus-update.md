---
title: termsAndConditionsAcceptanceStatus の更新
description: termsAndConditionsAcceptanceStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 886910cfe2ac0b1bcf6ad1fcbd0a76a79c515aba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858437"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="c4daf-103">termsAndConditionsAcceptanceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="c4daf-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="c4daf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4daf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4daf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4daf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4daf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c4daf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4daf-107">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c4daf-107">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c4daf-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c4daf-108">Prerequisites</span></span>
<span data-ttu-id="c4daf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4daf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4daf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4daf-111">Permission type</span></span>|<span data-ttu-id="c4daf-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4daf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4daf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4daf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4daf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4daf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c4daf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4daf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4daf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4daf-116">Not supported.</span></span>|
|<span data-ttu-id="c4daf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4daf-117">Application</span></span>|<span data-ttu-id="c4daf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4daf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4daf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4daf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="c4daf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4daf-120">Request headers</span></span>
|<span data-ttu-id="c4daf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4daf-121">Header</span></span>|<span data-ttu-id="c4daf-122">値</span><span class="sxs-lookup"><span data-stu-id="c4daf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4daf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4daf-123">Authorization</span></span>|<span data-ttu-id="c4daf-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c4daf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4daf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c4daf-125">Accept</span></span>|<span data-ttu-id="c4daf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4daf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4daf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4daf-127">Request body</span></span>
<span data-ttu-id="c4daf-128">要求本文で、[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c4daf-128">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="c4daf-129">次の表に、[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c4daf-129">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="c4daf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4daf-130">Property</span></span>|<span data-ttu-id="c4daf-131">種類</span><span class="sxs-lookup"><span data-stu-id="c4daf-131">Type</span></span>|<span data-ttu-id="c4daf-132">説明</span><span class="sxs-lookup"><span data-stu-id="c4daf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4daf-133">ID</span><span class="sxs-lookup"><span data-stu-id="c4daf-133">id</span></span>|<span data-ttu-id="c4daf-134">String</span><span class="sxs-lookup"><span data-stu-id="c4daf-134">String</span></span>|<span data-ttu-id="c4daf-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c4daf-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c4daf-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c4daf-136">userDisplayName</span></span>|<span data-ttu-id="c4daf-137">String</span><span class="sxs-lookup"><span data-stu-id="c4daf-137">String</span></span>|<span data-ttu-id="c4daf-138">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="c4daf-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="c4daf-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="c4daf-139">acceptedVersion</span></span>|<span data-ttu-id="c4daf-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c4daf-140">Int32</span></span>|<span data-ttu-id="c4daf-141">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="c4daf-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="c4daf-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4daf-142">acceptedDateTime</span></span>|<span data-ttu-id="c4daf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4daf-143">DateTimeOffset</span></span>|<span data-ttu-id="c4daf-144">最後にユーザーによって使用条件が承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c4daf-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="c4daf-145">応答</span><span class="sxs-lookup"><span data-stu-id="c4daf-145">Response</span></span>
<span data-ttu-id="c4daf-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c4daf-146">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4daf-147">例</span><span class="sxs-lookup"><span data-stu-id="c4daf-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="c4daf-148">要求</span><span class="sxs-lookup"><span data-stu-id="c4daf-148">Request</span></span>
<span data-ttu-id="c4daf-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4daf-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 138

{
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="c4daf-150">応答</span><span class="sxs-lookup"><span data-stu-id="c4daf-150">Response</span></span>
<span data-ttu-id="c4daf-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4daf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





