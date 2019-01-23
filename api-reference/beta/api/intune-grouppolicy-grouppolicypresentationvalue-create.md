---
title: GroupPolicyPresentationValue を作成します。
description: 新しい groupPolicyPresentationValue オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a6fbf02bdf9fb1c5d7f5fe5790943a956f2200c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430415"
---
# <a name="create-grouppolicypresentationvalue"></a><span data-ttu-id="22688-103">GroupPolicyPresentationValue を作成します。</span><span class="sxs-lookup"><span data-stu-id="22688-103">Create groupPolicyPresentationValue</span></span>

> <span data-ttu-id="22688-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="22688-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22688-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22688-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22688-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22688-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22688-107">新しい[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="22688-107">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22688-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="22688-108">Prerequisites</span></span>
<span data-ttu-id="22688-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22688-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="22688-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22688-111">Permission type</span></span>|<span data-ttu-id="22688-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="22688-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22688-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22688-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22688-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22688-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="22688-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22688-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22688-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22688-116">Not supported.</span></span>|
|<span data-ttu-id="22688-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22688-117">Application</span></span>|<span data-ttu-id="22688-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22688-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22688-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22688-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="22688-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22688-120">Request headers</span></span>
|<span data-ttu-id="22688-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22688-121">Header</span></span>|<span data-ttu-id="22688-122">値</span><span class="sxs-lookup"><span data-stu-id="22688-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22688-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22688-123">Authorization</span></span>|<span data-ttu-id="22688-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="22688-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22688-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22688-125">Accept</span></span>|<span data-ttu-id="22688-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22688-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22688-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="22688-127">Request body</span></span>
<span data-ttu-id="22688-128">要求の本文に groupPolicyPresentationValue オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="22688-128">In the request body, supply a JSON representation for the groupPolicyPresentationValue object.</span></span>

<span data-ttu-id="22688-129">次の表は、groupPolicyPresentationValue を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="22688-129">The following table shows the properties that are required when you create the groupPolicyPresentationValue.</span></span>

|<span data-ttu-id="22688-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22688-130">Property</span></span>|<span data-ttu-id="22688-131">型</span><span class="sxs-lookup"><span data-stu-id="22688-131">Type</span></span>|<span data-ttu-id="22688-132">説明</span><span class="sxs-lookup"><span data-stu-id="22688-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22688-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22688-133">lastModifiedDateTime</span></span>|<span data-ttu-id="22688-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22688-134">DateTimeOffset</span></span>|<span data-ttu-id="22688-135">日付と時刻オブジェクトが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="22688-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="22688-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22688-136">createdDateTime</span></span>|<span data-ttu-id="22688-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22688-137">DateTimeOffset</span></span>|<span data-ttu-id="22688-138">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="22688-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="22688-139">id</span><span class="sxs-lookup"><span data-stu-id="22688-139">id</span></span>|<span data-ttu-id="22688-140">String</span><span class="sxs-lookup"><span data-stu-id="22688-140">String</span></span>|<span data-ttu-id="22688-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="22688-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="22688-142">応答</span><span class="sxs-lookup"><span data-stu-id="22688-142">Response</span></span>
<span data-ttu-id="22688-143">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="22688-143">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22688-144">例</span><span class="sxs-lookup"><span data-stu-id="22688-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="22688-145">要求</span><span class="sxs-lookup"><span data-stu-id="22688-145">Request</span></span>
<span data-ttu-id="22688-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22688-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="22688-147">応答</span><span class="sxs-lookup"><span data-stu-id="22688-147">Response</span></span>
<span data-ttu-id="22688-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22688-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```




