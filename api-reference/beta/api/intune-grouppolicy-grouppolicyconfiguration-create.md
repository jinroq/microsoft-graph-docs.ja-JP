---
title: GroupPolicyConfiguration を作成します。
description: 新しい groupPolicyConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5ce3f8408d8a6e404ac17e865cc81bb2094c0cc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430538"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="48e0f-103">GroupPolicyConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="48e0f-103">Create groupPolicyConfiguration</span></span>

> <span data-ttu-id="48e0f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="48e0f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48e0f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48e0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48e0f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="48e0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48e0f-107">新しい[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="48e0f-107">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48e0f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="48e0f-108">Prerequisites</span></span>
<span data-ttu-id="48e0f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48e0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48e0f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48e0f-111">Permission type</span></span>|<span data-ttu-id="48e0f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="48e0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48e0f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48e0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48e0f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e0f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="48e0f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48e0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48e0f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48e0f-116">Not supported.</span></span>|
|<span data-ttu-id="48e0f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48e0f-117">Application</span></span>|<span data-ttu-id="48e0f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48e0f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48e0f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48e0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="48e0f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48e0f-120">Request headers</span></span>
|<span data-ttu-id="48e0f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48e0f-121">Header</span></span>|<span data-ttu-id="48e0f-122">値</span><span class="sxs-lookup"><span data-stu-id="48e0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48e0f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48e0f-123">Authorization</span></span>|<span data-ttu-id="48e0f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="48e0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48e0f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48e0f-125">Accept</span></span>|<span data-ttu-id="48e0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48e0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48e0f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="48e0f-127">Request body</span></span>
<span data-ttu-id="48e0f-128">要求の本文に groupPolicyConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="48e0f-128">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="48e0f-129">次の表は、groupPolicyConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="48e0f-129">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="48e0f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48e0f-130">Property</span></span>|<span data-ttu-id="48e0f-131">型</span><span class="sxs-lookup"><span data-stu-id="48e0f-131">Type</span></span>|<span data-ttu-id="48e0f-132">説明</span><span class="sxs-lookup"><span data-stu-id="48e0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e0f-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48e0f-133">createdDateTime</span></span>|<span data-ttu-id="48e0f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48e0f-134">DateTimeOffset</span></span>|<span data-ttu-id="48e0f-135">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="48e0f-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="48e0f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="48e0f-136">displayName</span></span>|<span data-ttu-id="48e0f-137">String</span><span class="sxs-lookup"><span data-stu-id="48e0f-137">String</span></span>|<span data-ttu-id="48e0f-138">リソース オブジェクトの名前をユーザーに提供されます。</span><span class="sxs-lookup"><span data-stu-id="48e0f-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="48e0f-139">説明</span><span class="sxs-lookup"><span data-stu-id="48e0f-139">description</span></span>|<span data-ttu-id="48e0f-140">String</span><span class="sxs-lookup"><span data-stu-id="48e0f-140">String</span></span>|<span data-ttu-id="48e0f-141">ユーザーは、リソース オブジェクトの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="48e0f-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="48e0f-142">id</span><span class="sxs-lookup"><span data-stu-id="48e0f-142">id</span></span>|<span data-ttu-id="48e0f-143">String</span><span class="sxs-lookup"><span data-stu-id="48e0f-143">String</span></span>|<span data-ttu-id="48e0f-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="48e0f-144">Key of the entity.</span></span>|
|<span data-ttu-id="48e0f-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48e0f-145">lastModifiedDateTime</span></span>|<span data-ttu-id="48e0f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48e0f-146">DateTimeOffset</span></span>|<span data-ttu-id="48e0f-147">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="48e0f-147">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="48e0f-148">応答</span><span class="sxs-lookup"><span data-stu-id="48e0f-148">Response</span></span>
<span data-ttu-id="48e0f-149">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="48e0f-149">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48e0f-150">例</span><span class="sxs-lookup"><span data-stu-id="48e0f-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="48e0f-151">要求</span><span class="sxs-lookup"><span data-stu-id="48e0f-151">Request</span></span>
<span data-ttu-id="48e0f-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="48e0f-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="48e0f-153">応答</span><span class="sxs-lookup"><span data-stu-id="48e0f-153">Response</span></span>
<span data-ttu-id="48e0f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48e0f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




