## ***[201801]*** Docker:Mysql:严格模式
> ***[20180110]*** 关闭严格模式
>> 修改.cnf配置文件
>> 
    # Copyright (c) 2016, Oracle and/or its affiliates. All rights reserved.
    #
    # This program is free software; you can redistribute it and/or modify
    # it under the terms of the GNU General Public License as published by
    # the Free Software Foundation; version 2 of the License.
    #
    # This program is distributed in the hope that it will be useful,
    # but WITHOUT ANY WARRANTY; without even the implied warranty of
    # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    # GNU General Public License for more details.
    #
    # You should have received a copy of the GNU General Public License
    # along with this program; if not, write to the Free Software
    # Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301 USA
    !includedir /etc/mysql/conf.d/
    !includedir /etc/mysql/mysql.conf.d/
    # 关闭严格模式
    [mysqld]
    sql_mode=NO_ENGINE_SUBSTITUTION,STRICT_TRANS_TABLES