---
title: GroupPolicyPresentationValueLongDecimal を作成する
description: 新しい groupPolicyPresentationValueLongDecimal オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4d95b26f07a5b575951415c697769c27989c188e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989029"
---
# <a name="create-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="caefb-103">GroupPolicyPresentationValueLongDecimal を作成する</span><span class="sxs-lookup"><span data-stu-id="caefb-103">Create groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="caefb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="caefb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caefb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="caefb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caefb-106">新しい[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="caefb-106">Create a new [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="caefb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="caefb-107">Prerequisites</span></span>
<span data-ttu-id="caefb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="caefb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caefb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="caefb-110">Permission type</span></span>|<span data-ttu-id="caefb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="caefb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caefb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="caefb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="caefb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caefb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="caefb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="caefb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caefb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="caefb-115">Not supported.</span></span>|
|<span data-ttu-id="caefb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="caefb-116">Application</span></span>|<span data-ttu-id="caefb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="caefb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="caefb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="caefb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="caefb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="caefb-119">Request headers</span></span>
|<span data-ttu-id="caefb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="caefb-120">Header</span></span>|<span data-ttu-id="caefb-121">値</span><span class="sxs-lookup"><span data-stu-id="caefb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caefb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="caefb-122">Authorization</span></span>|<span data-ttu-id="caefb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="caefb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="caefb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="caefb-124">Accept</span></span>|<span data-ttu-id="caefb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="caefb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caefb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="caefb-126">Request body</span></span>
<span data-ttu-id="caefb-127">要求本文で、groupPolicyPresentationValueLongDecimal オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="caefb-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueLongDecimal object.</span></span>

<span data-ttu-id="caefb-128">次の表に、groupPolicyPresentationValueLongDecimal の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="caefb-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueLongDecimal.</span></span>

|<span data-ttu-id="caefb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="caefb-129">Property</span></span>|<span data-ttu-id="caefb-130">型</span><span class="sxs-lookup"><span data-stu-id="caefb-130">Type</span></span>|<span data-ttu-id="caefb-131">説明</span><span class="sxs-lookup"><span data-stu-id="caefb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caefb-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="caefb-132">lastModifiedDateTime</span></span>|<span data-ttu-id="caefb-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caefb-133">DateTimeOffset</span></span>|<span data-ttu-id="caefb-134">オブジェクトが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="caefb-134">The date and time the object was last modified.</span></span> <span data-ttu-id="caefb-135">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="caefb-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="caefb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="caefb-136">createdDateTime</span></span>|<span data-ttu-id="caefb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caefb-137">DateTimeOffset</span></span>|<span data-ttu-id="caefb-138">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="caefb-138">The date and time the object was created.</span></span> <span data-ttu-id="caefb-139">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="caefb-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="caefb-140">id</span><span class="sxs-lookup"><span data-stu-id="caefb-140">id</span></span>|<span data-ttu-id="caefb-141">String</span><span class="sxs-lookup"><span data-stu-id="caefb-141">String</span></span>|<span data-ttu-id="caefb-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="caefb-142">Key of the entity.</span></span> <span data-ttu-id="caefb-143">[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="caefb-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="caefb-144">value</span><span class="sxs-lookup"><span data-stu-id="caefb-144">value</span></span>|<span data-ttu-id="caefb-145">Int64</span><span class="sxs-lookup"><span data-stu-id="caefb-145">Int64</span></span>|<span data-ttu-id="caefb-146">関連付けられたプレゼンテーションの符号なしの長整数型 (long) の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="caefb-146">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="caefb-147">応答</span><span class="sxs-lookup"><span data-stu-id="caefb-147">Response</span></span>
<span data-ttu-id="caefb-148">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="caefb-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caefb-149">例</span><span class="sxs-lookup"><span data-stu-id="caefb-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="caefb-150">要求</span><span class="sxs-lookup"><span data-stu-id="caefb-150">Request</span></span>
<span data-ttu-id="caefb-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="caefb-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="caefb-152">応答</span><span class="sxs-lookup"><span data-stu-id="caefb-152">Response</span></span>
<span data-ttu-id="caefb-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="caefb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "210f7078-7078-210f-7870-0f2178700f21",
  "value": 5
}
```





