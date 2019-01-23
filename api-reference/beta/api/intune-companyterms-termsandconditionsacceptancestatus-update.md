---
title: termsAndConditionsAcceptanceStatus の更新
description: termsAndConditionsAcceptanceStatus オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 548026bf033195364c0bda979f1501e62831ed13
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420543"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="6897a-103">termsAndConditionsAcceptanceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="6897a-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="6897a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6897a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6897a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6897a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6897a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6897a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6897a-107">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6897a-107">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6897a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6897a-108">Prerequisites</span></span>
<span data-ttu-id="6897a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6897a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6897a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6897a-111">Permission type</span></span>|<span data-ttu-id="6897a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6897a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6897a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6897a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6897a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6897a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6897a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6897a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6897a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6897a-116">Not supported.</span></span>|
|<span data-ttu-id="6897a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6897a-117">Application</span></span>|<span data-ttu-id="6897a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6897a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6897a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6897a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="6897a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6897a-120">Request headers</span></span>
|<span data-ttu-id="6897a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6897a-121">Header</span></span>|<span data-ttu-id="6897a-122">値</span><span class="sxs-lookup"><span data-stu-id="6897a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6897a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6897a-123">Authorization</span></span>|<span data-ttu-id="6897a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6897a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6897a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6897a-125">Accept</span></span>|<span data-ttu-id="6897a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6897a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6897a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6897a-127">Request body</span></span>
<span data-ttu-id="6897a-128">要求本文で、[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6897a-128">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="6897a-129">次の表に、[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6897a-129">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="6897a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6897a-130">Property</span></span>|<span data-ttu-id="6897a-131">型</span><span class="sxs-lookup"><span data-stu-id="6897a-131">Type</span></span>|<span data-ttu-id="6897a-132">説明</span><span class="sxs-lookup"><span data-stu-id="6897a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6897a-133">id</span><span class="sxs-lookup"><span data-stu-id="6897a-133">id</span></span>|<span data-ttu-id="6897a-134">String</span><span class="sxs-lookup"><span data-stu-id="6897a-134">String</span></span>|<span data-ttu-id="6897a-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6897a-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="6897a-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="6897a-136">userDisplayName</span></span>|<span data-ttu-id="6897a-137">String</span><span class="sxs-lookup"><span data-stu-id="6897a-137">String</span></span>|<span data-ttu-id="6897a-138">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="6897a-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="6897a-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="6897a-139">acceptedVersion</span></span>|<span data-ttu-id="6897a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6897a-140">Int32</span></span>|<span data-ttu-id="6897a-141">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="6897a-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="6897a-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="6897a-142">acceptedDateTime</span></span>|<span data-ttu-id="6897a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6897a-143">DateTimeOffset</span></span>|<span data-ttu-id="6897a-144">最後にユーザーによって使用条件が承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6897a-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="6897a-145">応答</span><span class="sxs-lookup"><span data-stu-id="6897a-145">Response</span></span>
<span data-ttu-id="6897a-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6897a-146">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6897a-147">例</span><span class="sxs-lookup"><span data-stu-id="6897a-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="6897a-148">要求</span><span class="sxs-lookup"><span data-stu-id="6897a-148">Request</span></span>
<span data-ttu-id="6897a-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6897a-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="6897a-150">応答</span><span class="sxs-lookup"><span data-stu-id="6897a-150">Response</span></span>
<span data-ttu-id="6897a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6897a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




