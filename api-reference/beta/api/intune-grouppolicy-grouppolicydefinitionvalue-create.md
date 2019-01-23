---
title: GroupPolicyDefinitionValue を作成します。
description: 新しい groupPolicyDefinitionValue オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d859a1405c9b2879da1c9b57f31c1ffde3ce0cfc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430357"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="b27fa-103">GroupPolicyDefinitionValue を作成します。</span><span class="sxs-lookup"><span data-stu-id="b27fa-103">Create groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="b27fa-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b27fa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b27fa-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b27fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b27fa-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b27fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b27fa-107">新しい[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b27fa-107">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b27fa-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b27fa-108">Prerequisites</span></span>
<span data-ttu-id="b27fa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b27fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b27fa-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b27fa-111">Permission type</span></span>|<span data-ttu-id="b27fa-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b27fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b27fa-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b27fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b27fa-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b27fa-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b27fa-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b27fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b27fa-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b27fa-116">Not supported.</span></span>|
|<span data-ttu-id="b27fa-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b27fa-117">Application</span></span>|<span data-ttu-id="b27fa-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b27fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b27fa-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b27fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="b27fa-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b27fa-120">Request headers</span></span>
|<span data-ttu-id="b27fa-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b27fa-121">Header</span></span>|<span data-ttu-id="b27fa-122">値</span><span class="sxs-lookup"><span data-stu-id="b27fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b27fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b27fa-123">Authorization</span></span>|<span data-ttu-id="b27fa-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b27fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b27fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b27fa-125">Accept</span></span>|<span data-ttu-id="b27fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b27fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b27fa-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b27fa-127">Request body</span></span>
<span data-ttu-id="b27fa-128">要求の本文に groupPolicyDefinitionValue オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b27fa-128">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="b27fa-129">次の表は、groupPolicyDefinitionValue を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b27fa-129">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="b27fa-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b27fa-130">Property</span></span>|<span data-ttu-id="b27fa-131">型</span><span class="sxs-lookup"><span data-stu-id="b27fa-131">Type</span></span>|<span data-ttu-id="b27fa-132">説明</span><span class="sxs-lookup"><span data-stu-id="b27fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b27fa-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b27fa-133">createdDateTime</span></span>|<span data-ttu-id="b27fa-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b27fa-134">DateTimeOffset</span></span>|<span data-ttu-id="b27fa-135">日付と時刻オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b27fa-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="b27fa-136">enabled</span><span class="sxs-lookup"><span data-stu-id="b27fa-136">enabled</span></span>|<span data-ttu-id="b27fa-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b27fa-137">Boolean</span></span>|<span data-ttu-id="b27fa-138">有効または、関連付けられているグループ ポリシーの定義を無効にします。</span><span class="sxs-lookup"><span data-stu-id="b27fa-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="b27fa-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="b27fa-139">configurationType</span></span>|[<span data-ttu-id="b27fa-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="b27fa-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="b27fa-141">値を構成する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="b27fa-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="b27fa-142">ポリシーとして、または環境設定のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="b27fa-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="b27fa-143">使用可能な値は、`policy`、`preference` です。</span><span class="sxs-lookup"><span data-stu-id="b27fa-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="b27fa-144">id</span><span class="sxs-lookup"><span data-stu-id="b27fa-144">id</span></span>|<span data-ttu-id="b27fa-145">String</span><span class="sxs-lookup"><span data-stu-id="b27fa-145">String</span></span>|<span data-ttu-id="b27fa-146">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b27fa-146">Key of the entity.</span></span>|
|<span data-ttu-id="b27fa-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b27fa-147">lastModifiedDateTime</span></span>|<span data-ttu-id="b27fa-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b27fa-148">DateTimeOffset</span></span>|<span data-ttu-id="b27fa-149">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="b27fa-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="b27fa-150">応答</span><span class="sxs-lookup"><span data-stu-id="b27fa-150">Response</span></span>
<span data-ttu-id="b27fa-151">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b27fa-151">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b27fa-152">例</span><span class="sxs-lookup"><span data-stu-id="b27fa-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b27fa-153">要求</span><span class="sxs-lookup"><span data-stu-id="b27fa-153">Request</span></span>
<span data-ttu-id="b27fa-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b27fa-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b27fa-155">応答</span><span class="sxs-lookup"><span data-stu-id="b27fa-155">Response</span></span>
<span data-ttu-id="b27fa-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b27fa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




