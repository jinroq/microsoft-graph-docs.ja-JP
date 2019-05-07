---
title: アプリの登録、アクセス許可、および同意移行の問題を確認する
description: Azure Active Directory (Azure AD) から Microsoft Graph API へのアプリの登録、アクセス許可、および同意の移行について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 54e187fcf35f030413aa98a6cb0e34649532a8b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630280"
---
# <a name="review-app-registration-permissions-and-consent"></a>アプリの登録、アクセス許可、同意を確認する

この記事は、「*手順 3:* アプリ[を移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の詳細を確認する」に含まれています。

アプリの更新プログラムには、次の3つの点を考慮する必要があります。

- **アプリの登録**: アプリケーションコードで既存のアプリの登録 (`appId`) を引き続き使用できます。  

    Microsoft Graph に移行するために、アプリを再登録する必要はあり**ません**。 コードを更新し、頻繁にテストして、更新プログラムを展開するだけです。  

- **アクセス許可**: アプリに対して構成済みの既存のアクセス許可を引き続き使用できます。 Azure AD Graph のアクセス許可は Microsoft Graph と共有されるため、新しいアクセス許可を要求する必要はありません。

    たとえば、既存のアプリに_ユーザー_が設定されている場合__ 、そのアクセス許可は、更新された Microsoft Graph のアプリに対して暗黙的に付与されます。

    更新プログラムで、Azure AD Graph で利用できない機能の使用が必要になった場合は、これらの新機能に対するアクセス許可を要求する必要があります。 その場合は、MSAL と v2 のエンドポイントを使用するようにアプリを切り替え、追加/増分の同意を動的に要求することができます。 「[アプリ認証ライブラリの変更を確認](/graph/migrate-azure-ad-graph-authentication-library)する」の「msal への切り替えの詳細」を参照してください。

- **同意**: エンドユーザーは、同意を再度付与するメッセージが表示されることなく、アプリを引き続き使用できます。

    自分のデータにアクセスするためにアプリに同意を付与しているユーザーは、再度同意を求められることなく、Microsoft Graph を使用するように更新された後もアプリを使用し続けることができます。

シンプルな移行プロジェクトでは、これらの領域で問題は発生しません。

ただし、新しい機能、サービス、またはその他の機能を使用する場合は、新しいアクセス許可とエンドユーザーの同意が必要になることがあります。  このような場合は、トークンの更新時に同意が要求されます。

## <a name="next-steps"></a>次のステップ

- Azure AD Graph と Microsoft Graph の[認証ライブラリ](migrate-azure-ad-graph-authentication-library.md)の違いについて説明します。
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。
