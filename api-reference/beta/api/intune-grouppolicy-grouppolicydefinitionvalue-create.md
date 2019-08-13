---
title: GroupPolicyDefinitionValue の作成
description: 新しい groupPolicyDefinitionValue オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 466b4bb57d1de402bfb56ee9553b735ac4116117
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355158"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="c6f39-103">GroupPolicyDefinitionValue の作成</span><span class="sxs-lookup"><span data-stu-id="c6f39-103">Create groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="c6f39-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6f39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6f39-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c6f39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6f39-106">新しい[Grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c6f39-106">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6f39-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c6f39-107">Prerequisites</span></span>
<span data-ttu-id="c6f39-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6f39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6f39-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c6f39-110">Permission type</span></span>|<span data-ttu-id="c6f39-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c6f39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6f39-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c6f39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6f39-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f39-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c6f39-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c6f39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6f39-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6f39-115">Not supported.</span></span>|
|<span data-ttu-id="c6f39-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c6f39-116">Application</span></span>|<span data-ttu-id="c6f39-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f39-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6f39-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c6f39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="c6f39-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6f39-119">Request headers</span></span>
|<span data-ttu-id="c6f39-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6f39-120">Header</span></span>|<span data-ttu-id="c6f39-121">値</span><span class="sxs-lookup"><span data-stu-id="c6f39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6f39-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6f39-122">Authorization</span></span>|<span data-ttu-id="c6f39-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c6f39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6f39-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c6f39-124">Accept</span></span>|<span data-ttu-id="c6f39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6f39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6f39-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c6f39-126">Request body</span></span>
<span data-ttu-id="c6f39-127">要求本文で、groupPolicyDefinitionValue オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c6f39-127">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="c6f39-128">次の表に、groupPolicyDefinitionValue の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c6f39-128">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="c6f39-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6f39-129">Property</span></span>|<span data-ttu-id="c6f39-130">型</span><span class="sxs-lookup"><span data-stu-id="c6f39-130">Type</span></span>|<span data-ttu-id="c6f39-131">説明</span><span class="sxs-lookup"><span data-stu-id="c6f39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6f39-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6f39-132">createdDateTime</span></span>|<span data-ttu-id="c6f39-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6f39-133">DateTimeOffset</span></span>|<span data-ttu-id="c6f39-134">オブジェクトが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c6f39-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="c6f39-135">enabled</span><span class="sxs-lookup"><span data-stu-id="c6f39-135">enabled</span></span>|<span data-ttu-id="c6f39-136">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="c6f39-136">Boolean</span></span>|<span data-ttu-id="c6f39-137">関連付けられたグループポリシー定義を有効または無効にします。</span><span class="sxs-lookup"><span data-stu-id="c6f39-137">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="c6f39-138">configurationType</span><span class="sxs-lookup"><span data-stu-id="c6f39-138">configurationType</span></span>|[<span data-ttu-id="c6f39-139">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="c6f39-139">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="c6f39-140">値の構成方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="c6f39-140">Specifies how the value should be configured.</span></span> <span data-ttu-id="c6f39-141">これは、ポリシーとして、または設定することができます。</span><span class="sxs-lookup"><span data-stu-id="c6f39-141">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="c6f39-142">可能な値は、`policy`、`preference` です。</span><span class="sxs-lookup"><span data-stu-id="c6f39-142">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="c6f39-143">id</span><span class="sxs-lookup"><span data-stu-id="c6f39-143">id</span></span>|<span data-ttu-id="c6f39-144">String</span><span class="sxs-lookup"><span data-stu-id="c6f39-144">String</span></span>|<span data-ttu-id="c6f39-145">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c6f39-145">Key of the entity.</span></span>|
|<span data-ttu-id="c6f39-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6f39-146">lastModifiedDateTime</span></span>|<span data-ttu-id="c6f39-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6f39-147">DateTimeOffset</span></span>|<span data-ttu-id="c6f39-148">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c6f39-148">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c6f39-149">応答</span><span class="sxs-lookup"><span data-stu-id="c6f39-149">Response</span></span>
<span data-ttu-id="c6f39-150">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c6f39-150">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6f39-151">例</span><span class="sxs-lookup"><span data-stu-id="c6f39-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6f39-152">要求</span><span class="sxs-lookup"><span data-stu-id="c6f39-152">Request</span></span>
<span data-ttu-id="c6f39-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c6f39-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="c6f39-154">応答</span><span class="sxs-lookup"><span data-stu-id="c6f39-154">Response</span></span>
<span data-ttu-id="c6f39-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c6f39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "enabled": true,
  "configurationType": "preference",
  "id": "50428918-8918-5042-1889-425018894250",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






