---
title: termsAndConditionsAcceptanceStatus の作成
description: 新しい termsAndConditionsAcceptanceStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f35721b273b9fe84afb21ff6b10bbb38d89a125f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255011"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="88aa9-103">termsAndConditionsAcceptanceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="88aa9-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="88aa9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88aa9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88aa9-105">新しい [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="88aa9-105">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88aa9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="88aa9-106">Prerequisites</span></span>
<span data-ttu-id="88aa9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88aa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88aa9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="88aa9-109">Permission type</span></span>|<span data-ttu-id="88aa9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="88aa9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88aa9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88aa9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88aa9-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88aa9-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="88aa9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88aa9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88aa9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88aa9-114">Not supported.</span></span>|
|<span data-ttu-id="88aa9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88aa9-115">Application</span></span>|<span data-ttu-id="88aa9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88aa9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88aa9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88aa9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="88aa9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88aa9-118">Request headers</span></span>
|<span data-ttu-id="88aa9-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88aa9-119">Header</span></span>|<span data-ttu-id="88aa9-120">値</span><span class="sxs-lookup"><span data-stu-id="88aa9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88aa9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="88aa9-121">Authorization</span></span>|<span data-ttu-id="88aa9-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="88aa9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88aa9-123">承諾</span><span class="sxs-lookup"><span data-stu-id="88aa9-123">Accept</span></span>|<span data-ttu-id="88aa9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88aa9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88aa9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="88aa9-125">Request body</span></span>
<span data-ttu-id="88aa9-126">要求本文で、termsAndConditionsAcceptanceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="88aa9-126">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="88aa9-127">次の表に、termsAndConditionsAcceptanceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="88aa9-127">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="88aa9-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88aa9-128">Property</span></span>|<span data-ttu-id="88aa9-129">型</span><span class="sxs-lookup"><span data-stu-id="88aa9-129">Type</span></span>|<span data-ttu-id="88aa9-130">説明</span><span class="sxs-lookup"><span data-stu-id="88aa9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88aa9-131">id</span><span class="sxs-lookup"><span data-stu-id="88aa9-131">id</span></span>|<span data-ttu-id="88aa9-132">文字列</span><span class="sxs-lookup"><span data-stu-id="88aa9-132">String</span></span>|<span data-ttu-id="88aa9-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="88aa9-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="88aa9-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="88aa9-134">userDisplayName</span></span>|<span data-ttu-id="88aa9-135">String</span><span class="sxs-lookup"><span data-stu-id="88aa9-135">String</span></span>|<span data-ttu-id="88aa9-136">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="88aa9-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="88aa9-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="88aa9-137">acceptedVersion</span></span>|<span data-ttu-id="88aa9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="88aa9-138">Int32</span></span>|<span data-ttu-id="88aa9-139">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="88aa9-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="88aa9-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="88aa9-140">acceptedDateTime</span></span>|<span data-ttu-id="88aa9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88aa9-141">DateTimeOffset</span></span>|<span data-ttu-id="88aa9-142">最後にユーザーによって使用条件が承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="88aa9-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="88aa9-143">応答</span><span class="sxs-lookup"><span data-stu-id="88aa9-143">Response</span></span>
<span data-ttu-id="88aa9-144">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="88aa9-144">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88aa9-145">例</span><span class="sxs-lookup"><span data-stu-id="88aa9-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="88aa9-146">要求</span><span class="sxs-lookup"><span data-stu-id="88aa9-146">Request</span></span>
<span data-ttu-id="88aa9-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="88aa9-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="88aa9-148">応答</span><span class="sxs-lookup"><span data-stu-id="88aa9-148">Response</span></span>
<span data-ttu-id="88aa9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="88aa9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



